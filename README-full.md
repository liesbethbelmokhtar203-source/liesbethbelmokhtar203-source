<p align="center">
  <img src="https://raw.githubusercontent.com/liesbethbelmokhtar203-source/liesbethbelmokhtar203-source/main/assets/header.svg" alt="Liesbeth Belmokhtar — Data Engineer" width="880"/>
</p>
<p align="center">
  <img src="https://raw.githubusercontent.com/liesbethbelmokhtar203-source/liesbethbelmokhtar203-source/main/assets/now.svg" alt="now" width="720"/>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/dbt-FF694B?style=flat&logo=dbt&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/Airflow-017CEE?style=flat&logo=apacheairflow&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/DuckDB-FFF000?style=flat&logo=duckdb&logoColor=black" height="22"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" height="22"/>
  <img src="https://img.shields.io/badge/Rust-000000?style=flat&logo=rust&logoColor=white" height="22"/>
</p>

---

Freelance data engineer in Antwerp. I build and repair analytics pipelines for
teams that do not have a data platform team.

Most weeks look the same: a dbt project that grew faster than its tests, an
Airflow DAG nobody wants to touch because the last person who did broke
finance's dashboard, a warehouse bill that doubled while everyone assumed
someone else was watching. That is the job. It is less interesting than the
conference talks make it sound and I like it anyway.

## What I work with

- **Modelling** dbt Core. SQL first, tests before dashboards, staging layer that
  does exactly one thing.
- **Orchestration** Airflow 2.x on most client stacks. Cron and a Makefile when
  the team is three people and Airflow would be the largest thing they run.
- **Warehouses** Postgres and DuckDB for local work, BigQuery and Snowflake where
  the client already lives.
- **Languages** SQL, Python (Polars more than pandas lately), Rust for the small
  command line things that need to start instantly.
- **Around it** Docker, dlt and Singer taps, Great Expectations, plain old make.
- **Editor** Neovim, mostly because retraining muscle memory is expensive.

## A few things here

**[dotfiles](https://github.com/liesbethbelmokhtar203-source/dotfiles)**
Shell setup I carry between machines. zsh and bash configs, the aliases I
actually use, and a `setup.sh` that symlinks them without eating whatever is
already in your home directory.

**[dbt-snippets](https://github.com/liesbethbelmokhtar203-source/dbt-snippets)**
Macros and model patterns I copy into every new dbt project. Dev row limits,
safe division, cents to euros in one place, and an incremental daily fact that
accounts for late-arriving rows.

**[csvstat](https://github.com/liesbethbelmokhtar203-source/csvstat)**
Small Rust CLI that prints per-column statistics for a CSV. Written because I
wanted to know whether a client export had nulls in the amount column, and I
did not want to wait for Python to import pandas to find out.

**[dbt-macro-pack](https://github.com/liesbethbelmokhtar203-source/dbt-macro-pack)**
A second bag of dbt macros — conditional not-null tests, accepted-range tests,
and an incremental helper that handles late-arriving rows by a lookback window.
The ones I reach for after dbt-snippets has done the basics.

**[dq-scan](https://github.com/liesbethbelmokhtar203-source/dq-scan)**
A tiny Python scanner that prints per-column data quality for a CSV — nulls,
duplicates, uniques, and a numeric summary when the column looks numeric. No
pandas, no dependencies, starts instantly. The thing I run first on every
client export before I trust it.

None of these are frameworks. They are the small tools that survived contact
with real projects, which is a lower bar than it sounds and also a real one.

## How I work

- Read the existing model before proposing a new one. Most pipelines are not
  badly designed, they are just undocumented.
- Tests go in with the model, not in a cleanup sprint that never gets scheduled.
- If a transformation cannot be explained to the person who owns the numbers, it
  is wrong, even when the output happens to be right.
- I would rather delete a model than add a column to it.

## 📊 Activity

<p align="center">
  <img height="160" src="https://github-readme-stats.vercel.app/api?username=liesbethbelmokhtar203-source&show_icons=true&theme=transparent&hide_border=true&count_private=true"/>
  <img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=liesbethbelmokhtar203-source&layout=compact&theme=transparent&hide_border=true"/>
</p>
<p align="center">
  <img width="720" src="https://github-readme-activity-graph.vercel.app/graph?username=liesbethbelmokhtar203-source&theme=github-compact&hide_border=true&radius=8"/>
</p>

## Notes

Client work stays in client repositories, so what is public here is deliberately
small. Everything I do publish is something I still use.

Written in English here, Dutch everywhere else. Documentation in either, on
request.

## Contact

Open an issue or a discussion on any repository above. That is the channel I
actually read. I do not do recruiter mail.

---

<sub>Antwerp, Belgium. CET/CEST. Coffee before 14:00, otherwise I am awake at 3
reading about columnar storage formats, which helps nobody.</sub>
