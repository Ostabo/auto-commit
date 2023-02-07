[![Auto commit](https://github.com/Ostabo/auto-commit/workflows/Auto%20commit/badge.svg)](https://github.com/Ostabo/auto-commit/actions?query=workflow%3A%22Auto+commit%22)

## Auto commit

This is a template for auto committing to GitHub using GitHub Actions.  
Check out the [workflow](.github/workflows/autocommit.yml) for more details.  
To configure cron job, check out [this](https://crontab.guru/) website.  

### Things to do:
1. Use this template
2. Replace usernames  
*autocommit.yml:*  
![Change yml](assets/tut-auto-commit-yml.png)  
*README.md:*  
![Change yml](assets/tut-auto-commit-readme.png)
3. Add GitHub Actions secret with your email  
![Add secret](assets/tut-auto-commit.png)  
4. Make sure GitHub Actions is allowed to read AND write to your repository  
*Settings > Actions > General > Workflow permissions*  
![Allow actions](assets/tut-auto-commit-permissions.png)  
5. GitHub Action will now run every day at 00:00 UTC and commit the current date to [*CURRENT_DATE*](https://github.com/Ostabo/auto-commit/blob/master/CURRENT_DATE) 

Note that GitHub Actions cron jobs might be delayed at high load times.

Action used: [GitHub Action for GitHub Push](https://github.com/ad-m/github-push-action)