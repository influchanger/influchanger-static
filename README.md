# influchanger-static

Emergency pages of influchanger.com, served by GitHub Pages at **https://status.influchanger.com/**, independent of the site (Heroku): the maintenance page « Le cap ne change pas », shown while the site is in maintenance or down.

- Heroku points `MAINTENANCE_PAGE_URL` and `ERROR_PAGE_URL` here.
- **Never edit these files by hand**: they are built in [influchanger-site](https://github.com/influchanger/influchanger-site) from `web/src/maintenance.src.html` and the brand tokens:
  ```bash
  cd influchanger-site && npm run static:publish -- ../influchanger-static
  cd ../influchanger-static && git add -A && git commit -m "Publish the emergency pages" && git push
  ```
- Public on purpose: no key, no data, no tracking. Decisions: [DECISIONS.md](DECISIONS.md) (G13, T01, T02).
