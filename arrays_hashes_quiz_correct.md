# Homework

### A. Given the following data structure:

```rb
lines = ['Gyle Centre', 'Edinburgh Park', 'Murrayfield Stadium', 'Haymarket', 'Princes Street']
```

1. Work out how many stops there are in the array
 puts lines.count
2. Return 'Edinburgh Park' from the array
puts lines[1]
3. How many ways can we return 'Princes Street' from the array?
lines[4] or lines[-1] or lines[lines.length()-1] or lines.last()
4. Work out the index position of 'Haymarket'
 puts lines.index("Haymarket")
5. Add 'Airport' to the start of the array
lines.unshift("Airport") lines.insert(0,"Airport")
6. Add 'York Place' to the end of the array
lines.push("York Place")
7. Remove 'Edinburgh Park' from the array using it's name
lines.delete("Edinburgh Park")
8. Delete 'Edinburgh Park' from the array by index
lines.delete_at(1)
9. Reverse the positions of the stops in the array
reversed_array = lines.reverse # creates a new array with the reversed order without replacing the original#
lines.reverse!()#replace the array#

### B. Given the following data structure:

```rb
  my_hash = {0 => "Zero", 1 => "One", :two => "Two", "two" => 2}
```

1. How would you return the string `"One"`?
puts my_hash[1] or my.hash.values_at(1)#you can put more than one index on this one#
2. How would you return the string `"Two"`?
 puts my_hash[:two]
3. How would you return the number `2`?
puts my_hash["two"]
4. How would you add `{3 => "Three"}` to the hash?
my_hash[3] = "Three"
my_hash[3] << "Three"
5. How would you add `{:four => 4}` to the hash?
my_hash[:four] = 4


### C. Given the following data structure:

```rb
  users = {
    "Jonathan" => {
      :twitter => "jonnyt",
      :favourite_numbers => [12, 42, 75, 12, 5],
      :home_town => "Stirling",
      :pets => {
        "fluffy" => :cat,
        "fido" => :dog,
        "spike" => :dog
      }
    },
    "Erik" => {
      :twitter => "eriksf",
      :favourite_numbers => [8, 12, 24],
      :home_town => "Linithgow",
      :pets => {
        "nemo" => :fish,
        "kevin" => :fish,
        "spike" => :dog,
        "rupert" => :parrot
      }
    },
    "Avril" => {
      :twitter => "bridgpally",
      :favourite_numbers => [12, 14, 85, 88],
      :home_town => "Dunbar",
      :pets => {
        "colin" => :snake
      }
    },
  }
```

1. Return Jonathan's Twitter handle (i.e. the string `"jonnyt"`)
 puts users["Jonathan"][:twitter]
2. Return Erik's hometown
puts users["Erik"][:home_town]
3. Return the array of Erik's favorite numbers
puts users["Erik"][:favourite_numbers]
4. Return the type of Avril's pet Colin
puts users["Avril"][:pets]["colin"]
5. Return the smallest of Erik's favorite numbers
puts users["Erik"][:favourite_numbers].min()

6. Add the number `7` to Erik's favorite numbers
users["Erik"][:favourite_numbers].push(7)# or unshift or shovel(<<) or insert#
7. Change Erik's hometown to Edinburgh
users["Erik"][:home_town]= "Edinburgh"
8. Add a pet dog to Erik called "Fluffy"
users["Erik"][:pets]["Fluffy"]= :dog
9. Add yourself to the users hash
users["Joao"] = {
  :twitter => "None",
  :favourite_numbers => [7, 3, 69],
  :home_town => "Lisbon",
  :pets => {
    "Tank" => :fish
  }
}
