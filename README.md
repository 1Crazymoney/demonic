# Demonic
*By Demonic-Coder*

Demonic is a library consisting of functions that make programming faster and clearer.

## Compiling

Demonic can be compiled with C ++ 14 standard.

## Installation

For the installation, you must first add the demonic folder to your project.

After that, you must also add the folder to your CMakeLists.txt file.<br>
`add_subdirectory(demonic)`

Next, you need to connect the library to your executable.<br>
`target_link_libraries(target demonic)`

## Usage

Here is a list of each function and its description and example.

#### string_in_string
Returns true if the specified `std::string` is part of the other specified `std::string`.<br>
`bool demonic::string_in_string("Cheese", "Cheesecake")`

#### string_has_char
Returns true if the indicated `char` is part of the indicated `std::string`.<br>
`demonic::string_has_char("abc", 'a')`

#### string_space
Places a `std::string` at the end of the number specified spaces.<br>
`demonic::string_space("my_string", 24)`

#### string_funnel
Creates a vector containing all possible `char` combinations<br>
`demonic::string_funnel("my_string")`

#### string_from_bash
Creates a `std::string` from the results of a bash-command.<br>
`std::string bash = demonic::string_from_bash("echo example")`

#### string_color
Creates a color `std::string` of the specified text, color, and style.<br>
`demonic::string_color("my_string", red, bold)`

#### string_highlight
Returns the specified part of a `std::string`, in the specified color and style.<br>
`demonic::string_highlight("my_string", blue, italic)`

#### string_lower
Creates a lowercase `std::string` from the specified `std::string`.<br>
`demonic::string_lower("MY_STRING")`

#### string_upper
Creates a uppercase `std::string` from the specified `std::string`.<br>
`demonic::string_upper("my_string")`

#### string_in_vector
A boolean that returns true if the specified `std::string` is part of the specified vector.<br>
`demonic::string_in_vector("my_string", vec)`

#### vector_from_string
Split the indicated `std::string` into a vector using the indicated `char` as a delimiter.<br>
`demonic::vector_from_string("a,b,c,d,e", ',')`

#### vector_from_bash
Creates a `std::vector<std::string>` of the specified bash command.<br>
`demonic::vector_from_bash("ls /home")`

#### vector_from_file
Creates a vector from the specified text file. By splitting the text every line<br>
`demonic::vector_from_file("/home/user/list.txt")`

#### vector_from_header
Grabs the corresponding list from the indicated header.<br>
`demonic::vector_from_header("[LIST]", "file.txt")`

#### helpmaker
A class that helps with creating a help output.<br>

#### true_rand
generates an actual random int.<br>
