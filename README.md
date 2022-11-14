## Laravel DynamoDB Demo

### Overview

This was a hands-on of using DynamoDB with Laravel and how it works/being configured

## Notes:
- The package being used is [baopham/laravel-dynamodb](https://github.com/kitar/laravel-dynamodb)
- `DYNAMODB_TABLE_PREFIX`: Can be used to group database tables (there's no databases on DynamoDB, only tables), so for example setting it as `LaravelDemo`:
  - Users table that has `protcted $table = 'Users`, would refer to `LaravelDemoUsers`  
  - Products table that has `protcted $table = 'Products`, would refer to `LaravelDemoProducts`  
- `DYNAMODB_ENDPOINT`: Correct value for your region can be brought from this [URL](https://docs.aws.amazon.com/general/latest/gr/ddb.html)
- There another package that is better matching Eloquent functions like `where`, `first`, ...etc. But it's a bit not maintained, it's [baopham/laravel-dynamodb](https://github.com/baopham/laravel-dynamodb)
  - Maybe both packages can be used simultaneously 