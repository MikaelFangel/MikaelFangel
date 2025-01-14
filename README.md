## Does it compile?
```fsharp
type PersonalInformation = { name: string; description: string; mail: string }
let myContactDetails =  {
    name = "Mikael Fangel"
    description = "I'm studying software engineering at DTU"
    mail = "public.tradition061@passinbox.com"
}

type Interest = string
let myInterest: Interest List = [ "Linux"; "Security"; "NixOS"; "Functional Programming" ]

type LevelOfConfidence = Advanced | Intermediate | Beginner
type SkillSet = { programmingLanguages: (LevelOfConfidence * string List) List
                  technologies: (LevelOfConfidence * string List) List }
let mySkillSet = {
    programmingLanguages = [
        (Advanced, [ "Java"; "Elixir"; "VBA" ])
        (Intermediate, [ "F#"; "Kotlin"; "C"; "C++" ])
        (Beginner, [ "R"; "Bash"; "Nix"; "Go"; "Prolog" ])
    ]
    technologies = [
        (Advanced, [ "Linux"; "Tines"; "Git" ])
        (Intermediate, [ "Docker"; "SIEM" ])
        (Beginner, [ "Firebase" ])
    ]
}

type URL = string
let myGist: URL = "https://gist.github.com/MikaelFangel"
```
