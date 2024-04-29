## Does it compile?
```fsharp
type PersonalInformation = { name: string; description: string; mail: string }
let myContactDetails =  {
    name = "Mikael Fangel"
    description = "I'm studying software engineering at DTU and I am currently doing an intership"
    mail = "public.tradition061@passinbox.com"
}

type Interest = string
let myInterest: Interest List = [ "Linux"; "Security"; "NixOS"; "Functional Programming" ]

type LevelOfConfidence = Advanced | Intermediate | Beginner
type SkillSet = { programmingLanguages: (LevelOfConfidence * string List) List
                  technologies: (LevelOfConfidence * string List) List }
let mySkillSet = {
    programmingLanguages = [
        (Advanced, [ "Java"; "C"])
        (Intermediate, [ "F#"; "Kotlin"; "Go"; "VBA" ])
        (Beginner, [ "R"; "Python"; "Bash"; "Awk"; "Nix"; "Elixir" ])
    ]
    technologies = [
        (Advanced, [ "Linux" ])
        (Intermediate, [ "Docker"; "SIEM" ])
        (Beginner, [])
    ]
}

type URL = string
let myGist: URL = "https://gist.github.com/MikaelFangel"
```
