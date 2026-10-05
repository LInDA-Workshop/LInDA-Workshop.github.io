# LInDA 2027 workshop website

Live site: https://linda-workshop.github.io/

Built with the [academicpages](https://github.com/academicpages/academicpages.github.io) template (Jekyll).

## Where to update what

| What to change | File |
|---|---|
| Home page, date, venue, About text | `_pages/about.md` |
| News | `_pages/news.md` |
| Program (sessions, times, chairs) | `_pages/program.md` |
| Invited speakers (titles, abstracts, bios) | `_pages/speakers.md` |
| Panel (panelists, moderator) | `_pages/panel.md` |
| Important dates | `_pages/dates.md` |
| Call for papers, submission links | `_pages/cfp.md` |
| Organizers and program committee | `_pages/committee.md` |
| Contact email, policy, sponsors | `_pages/contact.md` |
| Menu links (top bar and left sidebar) | `_data/navigation.yml` |
| Site title, URL, left sidebar text | `_config.yml` |

## How to edit

- Open the file and change the text between the HTML tags.
- Search for `TBA` to find missing details.
- Keep the tags (like `<p>` and `<td>`) in place.
- To add a menu item, create a page in `_pages/` and add it twice in `_data/navigation.yml` (once under `main`, once under `workshop`).
- Put images in `images/`.

## How to publish

1. Edit the file on GitHub (pencil icon) or locally.
2. Commit and push to the `main` branch.
3. Wait 2 to 5 minutes. The site updates by itself.
4. Check the build under the **Actions** tab if nothing changes.

## Preview locally (optional)

    bundle install
    bundle exec jekyll serve

Then open http://localhost:4000.

## Do not edit

Leave `_layouts/`, `_includes/`, and `_sass/` alone. They control the design.