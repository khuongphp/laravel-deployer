# Available recipes

Recipes are simple PHP files that you `require` in your `deploy.php`, to provide additional tasks and options. Whilst Laravel Deployer provides its own recipe — `recipe/laravel-deployer.php` — it also includes official recipes from Deployer that you can make use of.

## Recipes from deployphp/recipes

Deployer has an entire [github repository](https://github.com/deployphp/recipes) full of useful recipes.

To use any of them, simply add `require 'recipe/<recipe_name>.php'` to your `deploy.php` file and hook the provided tasks to existing tasks. Based on which recipe, you might also configure some options. Checkout the recipe's documentation provided by Deployer.org for more information.

| recipe name | description | |
| - | - | - |
| `bugsnag` | Enables you to send messages to Bugsnag. | [doc](https://github.com/deployphp/recipes/blob/master/docs/bugsnag.md) |
| `cachetool` | Clears APC system cach and resets the contents of the opcode cache. | [doc](https://github.com/deployphp/recipes/blob/master/docs/cachetool.md) |
| `cloudflare` | Clears cloudflare cache. | [doc](https://github.com/deployphp/recipes/blob/master/docs/cloudflare.md) |
| `hipchat` | Sends messages to hipchat. | [doc](https://github.com/deployphp/recipes/blob/master/docs/hipchat.md) |
| `newrelic` | Notifies New Relic of a new deployment. | [doc](https://github.com/deployphp/recipes/blob/master/docs/newrelic.md) |
| `npm` | **(included).** Install npm packages. Laravel Deployer already requires and extends this recipe to provide tasks that builds your assets. | [doc](https://github.com/deployphp/recipes/blob/master/docs/npm.md) |
| `phinx` | Migrate, rollback, run seeds and set a breakpoint for your database. | [doc](https://github.com/deployphp/recipes/blob/master/docs/phinx.md) |
| `rabbit` | Sends messages to rabbit. | [doc](https://github.com/deployphp/recipes/blob/master/docs/rabbit.md) |
| `rollbar` | Send messages to rollbar. | [doc](https://github.com/deployphp/recipes/blob/master/docs/rollbar.md) |
| `rsync` | Performs rsync from local `rsync_src` dir to remote `rsync_dest` dir and performs a warmup rsync on remote. | [doc](https://github.com/deployphp/recipes/blob/master/docs/rsync.md) |
| `sentry` | Sends messages to Sentry. | [doc](https://github.com/deployphp/recipes/blob/master/docs/sentry.md) |
| `slack` | Sends messages to slack including success and failure messages. | [doc](https://github.com/deployphp/recipes/blob/master/docs/slack.md) |
| `yammer` | Sends messages to yammer including success and failure messages. | [doc](https://github.com/deployphp/recipes/blob/master/docs/yammer.md) |
| `yarn` | Install Yarn packages. | [doc](https://github.com/deployphp/recipes/blob/master/docs/yarn.md) |
| `raygun` | Send deployment details to Raygun. | [doc](https://github.com/deployphp/recipes/blob/master/docs/raygun.md) |

## Framework recipes from deployphp/deployer

In case you're interested, Deployer also provides a handful of framework based recipes like Symfony, Magento, FuelPHP, etc. In fact, it also provides a Laravel recipe that Laravel Deployer is extending.