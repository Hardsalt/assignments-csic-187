# Big O Notation Questions and Answers

## Question 1
### Use Big O Notation to describe the time complexity of an algorithm that takes `4N + 16` steps.

## Answer 1
The time complexity is **O(N)** because we drop the constant coefficients.

---

## Question 2
### Use Big O Notation to describe the time complexity of an algorithm that takes `2N²`.

## Answer 2
The time complexity is **O(N²)** because constant multipliers are ignored in Big O notation.

---

## Question 3
### Use Big O Notation to describe the time complexity of the following function, which returns the sum of all numbers of an array after the numbers have been doubled.

```ruby
def double_then_sum(array)
    doubled_array = []

    array.each do |number|
        doubled_array << number *= 2
    end

    sum = 0

    doubled_array.each do |number|
        sum += number
    end

    return sum
end




def multiple_cases(array)
    array.each do |string|
        puts string.upcase
        puts string.downcase
        puts string.capitalize
    end
end

def every_other(array)
    array.each_with_index do |number, index|
        if index.even?
            array.each do |other_number|
                puts number + other_number
            end
        end
    end
end
