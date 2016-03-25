task "new" do
  counter = Dir["_posts/*.md"].last.split(/[-.]/)[-2].to_i + 1
  date = Time.now.strftime("%Y-%m-%d")
  filename = "_posts/#{date}-#{counter}.md"
  File.open(filename, "a+") do |f|
    f.puts "---"
    f.puts " layout: podcast"
    f.puts " title: Pai, ..."
    f.puts " podcast: #{counter}"
    f.puts " categories: [podcast]"
    f.puts " date: #{date}"
    f.puts " soundcloud: ?????"
    f.puts "---"
  end
  puts "vim #{filename}"
end