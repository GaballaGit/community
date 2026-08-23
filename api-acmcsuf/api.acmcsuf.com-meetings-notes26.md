## api meeting 3/14/26 summary:

### PR's merged over the week

- Databases migration is now done programatically, meaning manually doing
  `make migration-up/down` is no longer required
- The server now binds to localhost in dev mode, this is in preparation for
  deployment as api will have a different host name when in production
- Documents have been updated
- Swagger has been redirected to the `/docs` path now as we want to keep `/docs`
  as the source of truth for all documentation related to api
- The nix build has been simplified. Now the shell has the option to choose what
  dependencies it needs, speeding up the speed that ci runs

---

### PR's In progress

- huh CLI for events is now published, currently in the works by Josh
- Domain models is close to being ready for review. There are some nil pointer
  references that needed to be avoided in mapper first.
- Bipras is in the works of the script to populate the database

## api meeting 2/28/26 summary:

- Josh is taking on the refactor huh PR
- Gaballa is continuing to work on the domain and dto model refactor PR
- Tomas is currently looking into the logging and output issue
- Issue #165 has been opened for defining http.Client{} in the CLI

## api meeting 2/8/26 summary:

- Josh opened issues #148-156, which include refactoring sqlc and validating
  links in CLI forms
- Gaballa's PRs for DB migration and rate limiter have been merged, and he's now
  working on refactoring sqlc and huh
- Adam is also working on refactoring huh
- Sid updated the documentation and also made a layout for the workshop table,
  will be working on adding the schema

## api meeting 1/25/26 summary:

- Josh and Gaballa merged the CORS PR
- Josh is almost finished with the shorter microservice
- Gaballa brought up a problem with cobra flags in the huh library PR
- Gaballa also had an idea we can work on later for using the huh library as a
  full-on TUI
- The logging issue will likely be saved for new contributions
- Sid will be updating the documentation for new contributors
- The schedule for meetings might change after our first OS meeting, but likely
  not by much so that the four of us can still show up regularly

## api meeting 1/11/26 summary:

- Gaballa added the difficulty level tags for issues and is working on the CORS
  PR
- Sid is working on fixing unmarshaling in the db init script
