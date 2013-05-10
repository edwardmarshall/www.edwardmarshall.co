## Setup

Once you have cloned the repository, create a `.env` and `Procfile` in the root application directory.

Install foreman:
```
gem install foreman
```

Copy and paste the following code into your `Procfile`:
```
web: bundle exec unicorn -p $PORT -E $RACK_ENV -c ./config/unicorn.rb
```

Setup your `.env` file with the following config variables:
```
PORT=3000
RACK_ENV=development
ADMIN_MODE=false
```

Once the `.env` and `Procfile` are setup, you may run the server with the following command:
```foreman start```

## Questions

Send all application questions to Eric Taylor at [eric@edwardmarshall.co](mailto://eric@edwardmarshall.co).