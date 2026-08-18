# CV Template

A clean, single-page-friendly LaTeX CV/resume template. Fill in your own
details, compile to PDF, and you're ready to apply.

**[Download the example PDF](./example.pdf)** to see exactly what the
compiled output looks like — free to download and reuse, no sign-up required.

## Sections included

| Section | File | Notes |
|---|---|---|
| Heading (name, contact info) | `sections/heading.tex` | Pulled from `config.tex` |
| Education | `sections/education.tex` | Degree, institution, GPA, coursework |
| Professional Experience | `sections/experience.tex` | Work history with bullet points |
| Projects | `sections/projects.tex` | Personal/academic/hackathon projects |
| Volunteering & Organizational Experience | `sections/volunteering.tex` | Non-work leadership/community roles |
| Technical Skills | `sections/skills.tex` | Optional — toggle in `main.tex` |
| Achievements | `sections/achievements.tex` | Optional — toggle in `main.tex` |

Toggle any optional section on/off by commenting/uncommenting its
`\input{...}` line in `main.tex`.

## How it's organized

```
config.tex        -> your name/contact info (the only file most people need to edit)
preamble.tex       -> packages, formatting, reusable commands (rarely touched)
sections/*.tex      -> one file per CV section
main.tex             -> assembles everything, toggles optional sections
```

## Usage

1. Edit `config.tex` with your name, phone, email, GitHub, and LinkedIn.
2. Fill in each file under `sections/` with your own content.
3. Compile with `latexmk -pdf main.tex` (or open in [Overleaf](https://overleaf.com)).

## License

MIT — use it, modify it, share it.
