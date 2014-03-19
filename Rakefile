file "sublime-react" do |t|
  sh "git clone https://github.com/jgebhardt/sublime-react.git"
end

task :update => ["sublime-react"] do
  sh "cd sublime-react; git pull origin master; cd -"
end

def to_snippet(args)
  shortcut = args[:shortcut]
  body = args[:body]
  tabbed_body = body.gsub(/\n([^\n])/m, "\n\t\\1").strip
  "snippet #{shortcut}\n\t#{tabbed_body}"
end

def transform_snippet(filename)
  content = File.read(filename)
  /<tabTrigger>(?<shortcut>.*)<\/tabTrigger>/m =~ content
  /<!\[CDATA\[(?<body>.*)\]\]>/m =~ content
  
  to_snippet(shortcut: shortcut, body: body)
end

task :steal => [:update] do
  snippets = Dir.glob("sublime-react/snippets/*")
  transformed_snippets = snippets.map { |snippet| transform_snippet(snippet) }
  output = transformed_snippets.join("\n")
  File.open("snippets/javascript.snippets", "w") { |f| f.write(output) }

  puts "======================================================================"
  puts "Note: You should update rcc, the Sublime version doesn't work verbatim"
  puts "======================================================================"
end
