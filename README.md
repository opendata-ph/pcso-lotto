# pcso-lotto

![contributors](https://badgen.net/github/contributors/opendata-ph/pcso-lotto)
![stars](https://badgen.net/github/stars/opendata-ph/pcso-lotto)
![stars](https://badgen.net/github/forks/opendata-ph/pcso-lotto)
[![License](https://badgen.net/github/license/opendata-ph/pcso-lotto)](https://github.com/opendata-ph/pcso-lotto/blob/main/LICENSE)

A data collection of The Philippine Charity Sweepstakes Office (PCSO) lotto results.

## Data

### Description

PCSO is conducting five (5) major jackpot-bearing-games, four (4) major digit games and STL games in the Philippines. This data collection will aim to cover the results for the five (5) major jackpot-bearing-games namely:

- 6/58
- 6/55
- 6/49
- 6/45
- 6/42

### Structure

- The lotto result data will be presented in the following structure:

    ```json
    {
        "data": [
            {
                "date": "2022-12-08",
                "combination": "11-39-10-09-22-29",
                "prize": {
                    "amount": 10897597.6,
                    "currency": "PHP"
                }
            },
        ]
    }

    ```

    <table>
    <tr><th>Field</th><th>Data Type</th><th>Note</th></tr>
    <tr><td>date</td><td>Date</td><td>This follows ISO_LOCAL_DATE format, yyyy-MM-dd.</td></tr>
    <tr><td>combination</td><td>String</td><td>-</td></tr>
    <tr><td>prize.amount</td><td>Number</td><td>-</td></tr>
    <tr><td>prize.currency</td><td>String</td><td>-</td></tr>
    </table>

- The jackpot data will be presented in the following structure:

    ```json
    {
        "data": [
            {
                "date": "2022-12-11",
                "category": "6/49",
                "combination": "03-24-07-41-11-16",
                "prize": {
                    "amount": 23971499.6,
                    "currency": "PHP"
                },
                "winnerCount": 1
            }
        ]
    }

    ```

    <table>
    <tr><th>Field</th><th>Data Type</th><th>Note</th></tr>
    <tr><td>date</td><td>Date</td><td>This follows ISO_LOCAL_DATE format, yyyy-MM-dd.</td></tr>
    <tr><td>category</td><td>String</td><td>-</td></tr>
    <tr><td>combination</td><td>String</td><td>-</td></tr>
    <tr><td>prize.amount</td><td>Number</td><td>-</td></tr>
    <tr><td>prize.currency</td><td>String</td><td>-</td></tr>
    <tr><td>winnerCount</td><td>Number</td><td>-</td></tr>
    </table>

### Sources

The data was compiled using the following sources:

1. The Philippine Charity Sweepstakes Office (PCSO)
    * Links:
        * https://www.lottopcso.com/
        * https://www.lottopcso.com/6-58-lotto-result/
        * https://www.lottopcso.com/6-55-lotto-result/
        * https://www.lottopcso.com/6-49-lotto-result/
        * https://www.lottopcso.com/6-45-lotto-result/
        * https://www.lottopcso.com/6-42-lotto-result/

## Contributing

Pull requests and stars are always welcome. For additional data requests, please [create an issue](https://github.com/opendata-ph/pcso-lotto/issues/new).

1. Fork this repository and don't forget to star

2. Clone the repository

    ```bash
    $ git clone https://github.com/<your-username>/pcso-lotto.git
    ```

3. To keep your forked repository in sync with the upstream repository:

    ```bash
    $ git remote add upstream https://github.com/opendata-ph/pcso-lotto.git
    $ git fetch upstream
    $ git pull upstream main
    $ git push
    ```

4. Checkout to a new branch, preferred format would be:
   - For resolving issues
      - issue-<#>-<description>
   - For introducing new feature
      - feat-<description>
   - For minor fixes such as typos
      - chore-<description>
  
    ```bash
    # Branches are only a sample
    $ git checkout -b issue-1-memory-leak-fix
    $ git checkout -b feat-backend-implementation
    $ git checkout -b chore-minor-typo-fix
    ```

5. After changes has been made, add it to the staging area:

    ```bash
    $ git add -A
    $ git add <file>
    $ git add .
    ```

6. Commit the staged changes, and push it the branch created earlier:

    ```bash
    $ git commit -m <message>
    $ git push origin <branch-name>
    ```

7. Issue a pull request from forked repo to this repo by clicking on New Pull Request.

8. Fill in the title and provide a concise description.

9. Wait for respose on the Pull Request issued. 

10. Congratulations you just contributed to opensource!

## License

This repository is released under the [The Unlicense](https://github.com/opendata-ph/pcso-lotto/blob/main/LICENSE).