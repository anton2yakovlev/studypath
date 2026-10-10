# StudyPath

StudyPath turns a topic you want to learn into a realistic, time-boxed learning path built from real lessons. Tell Claude what you want to learn, how much time you have and what you already know. StudyPath maps the topic into modules, searches the learning platforms you have connected (Coursera, Udemy Business, O'Reilly) for the lectures, videos and labs that fit each module, vets them, checks the total time against your budget, and adds practice tasks and checkpoints. Afterwards it can write notes for any lesson, quiz you, turn the key facts into flashcards in Kuliko, and, only when you ask, schedule study sessions in Google Calendar or save the plan to Notion.

## Use it

Commands (in Cowork and Claude Code; in chat just describe what you want and Claude applies the matching skill):

- `/studypath:plan <topic>` - build a learning path, for example `/studypath:plan Rust ownership and borrowing, beginner, 4 weeks, 5 hours a week`
- `/studypath:notes <lesson link, course material or pasted transcript>` - structured notes with key ideas, examples and review questions
- `/studypath:practice <module or topic>` - quiz, flashcards and a spaced review schedule; flashcards go to Kuliko if it is connected
- `/studypath:save` - put the sessions on Google Calendar and/or export the plan to Notion, after you confirm a preview

Example prompts:

1. "Build me a 3-week plan to learn the basics of statistics from Coursera lessons, 4 hours a week, I know high-school algebra."
2. "I have Udemy Business through work. Make a 6-week path for Kubernetes for a backend developer, with labs."
3. "Make notes and a 10-question quiz for this lecture, put the flashcards in Kuliko, then schedule my review sessions next week after 6 pm."

## Connectors

The plugin lists six directory connectors. Every one is optional; connect only the ones you use from the plugin's Connectors tab.

| Connector | What StudyPath uses it for |
| - | - |
| Coursera | Search courses, short videos and hands-on projects; read course material for notes |
| Udemy Business | Search lectures, courses, learning paths and labs; read a course curriculum |
| O'Reilly | Search books, video courses and live events |
| Kuliko | Create a subject and flashcards for spaced repetition |
| Google Calendar | Find free slots and create study sessions |
| Notion | Export the finished plan as a page |

Coursera, Udemy Business and O'Reilly need an account on that platform; some content needs a subscription or an employer licence. With none of the learning platforms connected, StudyPath still builds a plan from links you provide and from web search when it is enabled in your Claude settings, including YouTube and university open-courseware pages. For a public video the plugin can read only what the page shows (title, description, chapters); paste a transcript for timestamped notes.

## Data and privacy

StudyPath has no server and stores nothing. It sends your topic and search terms to the connectors and search tools you have enabled. Google Calendar is read only inside the time window you ask for and only to find free slots. Events, pages and flashcards are created only after you confirm a preview, and the plugin never edits or deletes anything that already exists. It does not read your email and does not use Claude's memory or past chats for personalization. Lesson text, descriptions and web pages are treated as untrusted data, never as instructions.

## Limitations

Plans are only as good as the sources Claude can reach. StudyPath never invents lessons or links: it lists only what it found or what you supplied, and says when it could not confirm a source. For medical, legal, tax or investment topics the plan is general education, not personal advice. Notes paraphrase; they quote at most one short phrase per lesson.

## Trademarks

StudyPath is an independent project. It is not affiliated with or endorsed by Coursera, Udemy, O'Reilly, Kuliko, Google, Notion, YouTube or Anthropic. All product names belong to their owners.

## License

MIT, see the LICENSE file.
