1〜30までの数字の中で<br>
3の倍数の時はFizz<br>
5の倍数の時はBuzz<br>
を出力します。<br>
aの倍数という表現は、ある数字numをaで割った時の余が0であるという書き方で求めることができます。

#### 例1
- **rubyの場合**
```ruby
for num in 1..30 do
  if num % 3 == 0 && num % 5 == 0
    puts "#{num}:FizzBuzz"
  elsif num % 3 == 0
    puts "#{num}:Fizz"
  elsif num % 5 == 0
    puts "#{num}:Buzz"
  else
    puts num
  end
end
# 1
# 2
# 3:Fizz
# 4
# 5:Buzz
# .
# .
# .
# 28
# 29
# 30:FizzBuzz
```
#### 例2
- **rubyの場合**
```ruby
for num in 1..30 do
  output = ""
  if num % 3 == 0
    output = "Fizz"
  end
  if num % 5 == 0
    output = output + "Buzz"
  end
  puts "#{num}:#{output}"
end
# 1:
# 2:
# 3:Fizz
# 4:
# 5:Buzz
# .
# .
# .
# 28:
# 29:
# 30:FizzBuzz
```
