<!--START_SECTION:waka-->

name: Kissinger156

on:
  schedule:
    # Runs at 12am IST
    - cron: '30 18 * * *'
    workflow_dispatch:
jobs:
  update-readme:
    name: Update Readme with Metrics
    runs-on: ubuntu-latest
    steps:
      - uses: kissinger156/README.md@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
          GH_TOKEN: ${{ secrets.GH_TOKEN }}

<!--END_SECTION:waka-->
