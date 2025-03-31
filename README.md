<a href="https://stackoverflow.com/users/4417582/abhimanyuaryan"><img src="https://stackoverflow.com/users/flair/4417582.png?theme=dark" width="208" height="58" alt="profile for abhi at Stack Overflow, Q&amp;A for professional and enthusiast programmers" title="profile for abhi at Stack Overflow, Q&amp;A for professional and enthusiast programmers"></a>

# Hi there, I'm Abhimanyu Aryan 👋 - call me (Aryan/Abhi)

# Current hobby projects
- Working with BAML to improve accuracy of response: https://www.promptfiddle.com/
- Testing AG2 RAG 

I'm a computer scientist with a passion for Julia programming and a love for a wide range of activities. Here's a bit about me:

## 🙋‍♂️ About Me
```julia
using Dates

Base.@kwdef struct AbhimanyuAryan
    job👔::String = "computer scientist"
    bdate📅::Date = Date(1995, 9, 13)
    website🌐::String = "https://abhimanyuaryan.com"
    current_projects🛠️::Vector{String}
    hobbies🎉::Vector{String} = ["dance", "gym", "football", "table tennis", "lawn tennis", "swimming", "boxing", "computer games", "hacking", "almost anything that gets my adrenaline up"]
end

age(a::AbhimanyuAryan) = Dates.year(now()) - Dates.year(a.bdate📅)
Base.summary(a::AbhimanyuAryan) = "Some $(age(a)) year old $(a.job👔)"
workson(a::AbhimanyuAryan) = a.current_projects🛠️

me = AbhimanyuAryan(current_projects🛠️ = [
    "Genie.jl",
    "Stipple.jl (plotly, ui)",
    "SearchLight.jl"
])

println(summary(me))
println("works on: $(join(me.current_projects🛠️, ', '))")
println("has hobbies: $(join(me.hobbies🎉, ', '))")
```

As an open-source contributor, I am enthusiastic about building a reliable web ecosystem that facilitates the work of data scientists, researchers, and machine learning practitioners. Passionate about the intersection of EdTech, Large Language Models (LLMs), and cloud technologies, I embarked on my journey in India's leading EdTech sector, advocating for self-driven education over traditional models for scalable learning. Currently, I am deeply exploring the potential of LLMs and AI, driven by a vision to revolutionize how we learn and interact with technology.

```julia
struct EuropeMap
    map::Array{String,1}
    home_country::String
end

function show_home(map::EuropeMap)
    for line in map.map
        println(line)
    end
    println("\njulia> where abhimanyu lives")
    println("        Home: ", map.home_country)
end

eu = EuropeMap([
    "        +----+          +----+",
    "        |UK  |          |NOR |",
    "  +-----+----+----+     +----+",
    "  |IRE  |FR  |GER |",
    "  |     +----+    |",
    "  |PT   |SP* |    |     +----+",
    "  +-----+----| IT |-----|POL |",
    "        |    |    |     +----+",
    "        |GRE |    |",
    "        +----+----+"
], "some where in 🇪🇺")

show_home(eu)
```
