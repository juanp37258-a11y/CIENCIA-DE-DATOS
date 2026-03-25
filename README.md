# .github/workflows/readme.yml
name: Update README
on: [push]
jobs:
  update:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - run: |
          echo "# Mi Proyecto" > README.md
          echo "" >> README.md
          echo "## Estructura de archivos" >> README.md
          echo '```' >> README.md
          find . -not -path './.git/*' | sort >> README.md
          echo '```' >> README.md
      - uses: stefanzweifel/git-auto-commit-action@v4
        with:
          commit_message: "docs: update README file structure"
