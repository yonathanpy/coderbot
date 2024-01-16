import requests
from github import Github

# Replace these with your own GitHub token and repository information
github_token = 'YOUR_GITHUB_TOKEN'
repository_owner = 'owner'
repository_name = 'repo'
issue_number = 1  # Replace with the actual issue number

# Initialize the GitHub API client
github_client = Github(github_token)
repository = github_client.get_repo(f"{repository_owner}/{repository_name}")
issue = repository.get_issue(issue_number)

# Comment on the issue
def comment_on_issue(comment_body):
    issue.create_comment(comment_body)

# Example comment
comment_body = "Hello, this is a comment from the bot!"
comment_on_issue(comment_body)
