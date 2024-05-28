## Does it compile?
```gleam
pub type PersonalInformation { PersonalInformation(name: String, description: String, mail: String) }
pub fn my_contact_details() -> PersonalInformation {
  PersonalInformation(
    name: "Mikael Fangel",
    description: "I'm studying software engineering at DTU",
    mail: "public.tradition061@passinbox.com",
  )
}

pub type Interest = String
pub fn my_interst() -> List(Interest) {
  ["Linux", "Security", "NixOS", "Functional Programming"]
}

pub type LevelOfConfidence { Advanced Intermediate Beginner }
pub type SkillSet {
  SkillSet(programming_languages: List(#(LevelOfConfidence, List(String))),
           technologies: List(#(LevelOfConfidence, List(String))),)
}
pub fn my_skill_set() -> SkillSet {
  SkillSet(
    programming_languages: [
      #(Advanced, ["Java", "C"]),
      #(Intermediate, ["F#", "Kotlin", "Go", "VBA"]),
      #(Beginner, ["R", "Python", "Bash", "Awk", "Nix", "Elixir", "Gleam"]),
    ],
    technologies: [
      #(Advanced, ["Linux"]),
      #(Intermediate, ["Dokcer", "SIEM"]),
      #(Beginner, []),
    ],
  )
}

pub type URL = String
pub fn my_gist() -> URL {
  "https://gist.github.com/MikaelFangel"
}
```
