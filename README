A simple buildpack that simply curls a URL defined in `BUILDPACK_WEBHOOK_URL`.

Useful for Gigalixir or Heroku if you want to notify some other service about each deploy.

To add this buildpack to Gigalixir, you need a `.buildpacks` file. For example, if you are using mix

    https://github.com/gigalixir/gigalixir-buildpack-clean-cache.git
    https://github.com/HashNuke/heroku-buildpack-elixir
    https://github.com/gjaldon/heroku-buildpack-phoenix-static
    https://github.com/gigalixir/gigalixir-buildpack-mix.git
    https://github.com/jesseshieh/buildpack-webhook.git

Then set the url to curl, for example

    gigalixir config:set -a $APP_NAME BUILDPACK_WEBHOOK_URL="https://www.google.com"

If you need to customize the curl command or need extra information like the current sha, 
feel free to send over a pull request and/or fork this and add your fork to your `.buildpacks` file.

