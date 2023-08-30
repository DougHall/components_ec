# ElixirConf Breakdown: LiveView Components 2023
Groxio LiveView Components Course

## 1 Install these tools, plus Elixir, plus Phoenix. 

The tools you will need to install: 

- git (https://git-scm.com/downloads). 
- an editor that you are comfortable with. 
- a working PostgreSQL install

For the development dependencies, you'll need: 

- Elixir 1.15, with OTP 26. Make sure it's working: 

run the command: 

```
[course] ➔ elixir -v
Erlang/OTP 26 [erts-14.0.2] [source] [64-bit] [smp:10:10] [ds:10:10:10] [async-threads:1] [jit]

Elixir 1.15.4 (compiled with Erlang/OTP 26)
```

- Phoenix 1.7.7. This version of Phoenix is significantly different than previous ones.


Is Phoenix working? Make sure you can run this command: 

```
mix phx.new demo
(say yes to fetch dependencies and assets)
```

and make sure you can then create the database: 

```
cd demo
mix ecto.create
```

Don't save this for the last minute! There are a few dependencies that will give you trouble if you've never done this before and decide to wait. 


## 2. Clone this repository

1. Fork this repository to your github account. 

- Go to https://github.com/groxio-learning/components_ec_remote
- Click the `fork` button in the upper right corner
- Navigate to *your local version* (at something like git@github.com:your-github-user/components_ec_remote.git. )
- Copy the clone address to your clipboard. In the upper right, click `clone or download` then `copy to clipboard`

2. Clone your local version to your local machine. 

- Clone it. *REPLACE your-github-account with your account*:  

```
>  git clone <paste the url>
...clones repo...
cd components_ec_remote
```

- Verify your remote: 

```
$ git remote -v
> origin  https://github.com/your-user/components_ec_remote.git (fetch)
> origin  https://github.com/your-user/components_ec_remote.git (push)
```


- If there's no origin, set it. Make sure you *replace your-github-user*:

```
components_ec_remote> git remote add origin https://github.com/your-github-user/components_ec_remote.git
```

- Verify your remote: 

```
$ git remote -v
> origin  https://github.com/your-user/components_ec_remote.git (fetch)
> origin  https://github.com/your-user/components_ec_remote.git (push)
```

- Set the upstream to the Groxio repo:

```
components_ec_remote> git remote add upstream https://github.com/groxio-learning/components_ec_remote.git
```

- Verify the remotes: 

```
> origin  https://github.com/your-user/components_ec_remote.git (fetch)
> origin  https://github.com/your-user/components_ec_remote.git (push)
> upstream  https://github.com/groxio-learning/components_ec_remote.git (fetch)
> upstream  https://github.com/groxio-learning/components_ec_remote.git (push)
```

3. Now check out your setup. Send me a pull request: Edit the file "pull_requests.md" and add your name: 

- git pull upstream main
- Edit pull_requests.md

```
- Bruce Tate
```

- Commit the file and push

```
> git commit . -m "my commit"

...some happy success message...

> git push origin main

...some happy success message...
```

Now go to _your repo_ in your browser. Navigate to pull requests, and create the button to create a pull request. 

Your homework is done!
