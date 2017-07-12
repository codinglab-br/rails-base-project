# Rails Base Project
You can use this project as a quick start for your new Rails project. It was created using Rails 5.1.2 (Ruby 2.3.4), PostgreSQL and RSpec.

It also features the following gems:
- [factory_girl_rails](https://github.com/thoughtbot/factory_girl_rails)
- [shoulda_matchers](https://github.com/thoughtbot/shoulda-matchers)
- [rubocop](https://github.com/bbatsov/rubocop)
- [simplecov](https://github.com/colszowka/simplecov)

#### Setup
To start using this, create a new repository (GitHub, GitLab, etc) and download this base project from [here](https://github.com/grascovit/rails-base-project/archive/master.zip). Extract the downloaded file and rename the folder to your new project name.

Run the following commands inside the root folder to setup your new project:
```shell
git init
git remote add origin your-project-git-url
bundle install
```

Then, make a copy of the `application.yml.example` file located in the `config` folder and rename the new file to `application.yml` and insert your PostgreSQL data (no quotes needed):
```shell
DATABASE_NAME: your-project-name
DATABASE_USERNAME: your-postgres-username
DATABASE_PASSWORD: your-postgres-password
```

After this, execute the following step:
```shell
rake db:create
```
Finally, run the application:
```shell
rails s
```

Don't forget to update this `README.md` to whatever your want before pushing.