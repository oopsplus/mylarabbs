#Some Guide For Setting Up <b><em>larabbs</em></b>

## Step 1
Setup Homestead. See:
https://learnku.com/docs/laravel-development-environment/5.7

Note:
- On windows, when running the `vagrant up` command in the cmd or gitbash and etc, 
  make sure the cmd or gitbash and etc is running as Administrator. You can run
  `net session` in those shells to check weather the shell is in Administrator mode. 

- Maybe the box downloading is very slow. And Maybe I can package one for you on my
  personal computer. When use the packed box, please refer to the `vagrant add --help`
  command when adding the packed box.

- You can ask me for some basic setup info for the `.env` file.

## Step 2
Run `composer install` to install the php packages used by the laravel framework and
our application.


## Step 3
Run `yarn install` to install the dependent npm package for front-end developing flow.


## Step 4
Run `npm run dev` to generate the front-end assets for the application. 


## Step 5
Run `artisan migrate` to start database migration.

If you'd like to see some faking seeding data when in development environment, please
run `artisian migrate --seed`. DON'T RUN IT WHEN IN PRODUCTION ENVIRONMENT.


## Step 6
configure 
```
192.168.10.10  larabbs.test
```
in your hosts file.
- Windows: C:\Windows\System32\drivers\etc\hosts
- Mac&Linux: /etc/hosts

## Step 7
Open http://larabbs.test in your favorite browser.
