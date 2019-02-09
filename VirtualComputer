class Computer
	@@users = {}
  
  def initialize(username, password)
    @username = username
    @password = password
    @files = {}
    @@users[username] = password
  end
  
  def create(filename)
    time = Time.now
    @files[filename] = time
    puts "#{filename} was created by #{@username} at #{time}."
  end
  
  def Computer.get_users
    @@users
  end
end

my_computer = Computer.new("tom",36784)
your_computer = Computer.new("you", 26842)

my_computer.create("planets.txt")
your_computer.create("list.txt")

puts "Users: #{Computer.get_users}"
