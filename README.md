# Docker's Birthday Site

We are happy to accept contributions to our Birthday party site.  Read this page
if you want to contribute or to [publish the site](#publish-the-site).


## Quickstart Contributors

* [Get set up](#get-set-up)
* [Set your signature and an upstream remote](#set-your-signature-and-an-upstream-remote)
* [Make changes on a feature branch](#make-changes-on-a-feature-branch)
* [Rebase your branch](#rebase-your-branch)
* [Create a pull request](#create-a-pull-request)

### Get set up

Before you begin, [install Hugo](http://goo.gl/QDR7zf); this allows you to test
your changes locally. Then:

1. Fork this repository.

	Use the **Fork** button this page.
	
2. Copy your fork's clone URL from GitHub.

  GitHub allows you to use HTTPS or SSH protocols for clones. You can use the
  `git` command line or clients like Subversion to clone a repository. These
  instructions assume you are using the HTTPS protocol and the `git` command
  line. 

3. Clone the fork to your local machine.

		git clone https://github.com/moxiegirl/birthdaysite.git
		
		
### Set your signature and an upstream remote

When you contribute to Docker, you must certify you agree with the 
<a href="http://developercertificate.org/" target="_blank">Developer Certificate of Origin</a>.
You indicate your agreement by signing your `git` commits like this:

    Signed-off-by: Pat Smith <pat.smith@email.com>

To create a signature, you configure your username and email address in Git.
You can set these globally or locally on just your `birthdaysite` repository.
You must sign with your real name. We don't accept anonymous contributions or
contributions through pseudonyms.

As you change code in your fork, you'll want to keep it in sync with the changes
others make in the `docker/birthdaysite` repository. To make syncing easier, you'll
also add a _remote_ called `upstream` that points to `docker/birthdaysite`. A remote
is just another a project version hosted on the internet or network.

To configure your username, email, and add a remote:

1. Change to the root of your `birthdaysite` repository.

        $ cd birthdaysite

2. Set your `user.name` for the repository.

        $ git config --local user.name "FirstName LastName"

3. Set your `user.email` for the repository.

        $ git config --local user.email "emailname@mycompany.com"

4. Set your local repo to track changes upstream, on the `docker` repository. 

        $ git remote add upstream https://github.com/docker/birthdaysite.git

5. Check the result in your `git` configuration.

        $ git config --local -l

	To list just the remotes use:

        $ git remote -v

## Make changes on a feature branch

1. Change to the root of your local fork.

2. Create a feature branch.

			$ git checkout -b my-keen-feature
		
3. Start Hugo so you can see your changes as you work.

	To do this, you run Hugo locally. From the root of your local repo:
	
			$ hugo server -w

4. Begin making changes in your feature branch.

5. When you are done, check the status of your branch. 

			$ git status
        
6. Add your changes file with `git add` command.

7. Sign and commit your change.

			$ git commit -s -m "Adding some super changes."

  Commit messages should have a short summary sentence of no more than 50
  characters. Optionally, you can also include a more detailed explanation after
  the summary. Separate the summary from any explanation with an empty line.

8. Push your changes to GitHub.

			$ git push --set-upstream origin my-keen-feature
			Username for 'https://github.com': moxiegirl
			Password for 'https://moxiegirl@github.com': 

    Git prompts you for your GitHub username and password. Then, the command
    returns a result.

9. Open your browser to Github.

10. Navigate to your `birthdaysite` fork.

11. Make sure the `my-keen-feature` branch exists, that it has your commit, and the
commit is signed.


## Rebase your branch

Always rebase and squash your commits before making a pull request. 

1. Fetch any of the last minute changes from `docker/birthdaysite`.

        $ git fetch upstream master

3. Start an interactive rebase.

        $ git rebase -i upstream/master

4. Rebase opens an editor with a list of commits.

		pick 1a79f55 Tweak some of images
		pick 3ce07bb Add a new line 
        
  If you run into trouble, `git --rebase abort` removes any changes and gets you
  back to where you started. 

4. Squash the `pick` keyword with `squash` on all but the first commit.

		pick 1a79f55 Tweak some of images
		squash 3ce07bb Add a new line 

	After closing the file, `git` opens your editor again to edit the commit
	message. 

5. Edit and save your commit message.

	`git commit -s`

 Make sure your message includes your signature.

8. Push any changes to your fork on GitHub.

        $ git push origin my-keen-feature
        
## Create a pull request 

1. Open your browser to your fork on GitHub.

    You should see the latest activity from your branch.

2. Click "Compare & pull request."

    The system displays the pull request dialog. The pull request compares your
    changes to the `master` branch on the `docker/birthdaysite` repository.

3. Edit the dialog's description and add a reference to the issue you are fixing.

    GitHub helps you out by searching for the issue as you type.

4. Scroll down and verify the PR contains the commits and changes you expect.

    For example, is the file count correct? Are the changes in the files what
    you expect.

5. Press "Create pull request".

    The system creates the request and opens it for you in the `docker/birthdaysite`
    repository.

6. Participate in the PR review.


## Publish the site 

This is for site owners:

1. Get the keys from @spf13 or @moxiegirl or Jess.

2. Make and push master.

	```console
	$ AWS_S3_BUCKET=docker.party  AWS_ACCESS_KEY="AKI....7Q5A" AWS_SECRET_KEY="w1Gq...LHb67..Xy3Mi"  make
	```
