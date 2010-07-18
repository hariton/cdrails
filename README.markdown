Bash-script for quick upfloat from the Rails subdirectories to RAILSROOT.
It can be useful to those who constantly live in the console.

# Using

Place `cdrails` in any dir included in your $PATH.

deep diving (standard Spree-directory):

`cd vendor/extensions/site/app/views`

quick surface

`. cdrails`

For convenience possible to make alias and link, something like:

`alias cdr=cdrails`

`ln -s cdrails cdr`

And then:

`. cdr`

It is also possible to jump to Rails-dir without any '../../..', for example:

  `cd vendor/extensions/site/app/views`

  `. cdr app/views/layouts`

Or to special Rails-shortcats:

  `. cdr migrate`

  `. cdr plugins`

  etc.

List of shortcats:

- models -> app/models
- controllers -> app/controllers
- helpers -> app/helpers
- views -> app/views
- layouts -> app/views/layouts
- migrate -> db/migrate
- gems -> vendor/gems
- plugins -> vendor/plugins

---------------------------------------

For details, see code and `man bash` (about `source`):

> Read and execute commands from filename in the current shell
> environment and return the exit  status  of  the last  command
> executed  from filename.

## See also

- [cdgem](http://gist.github.com/478223) - cli gem navigation
- ["Cdrails - быстрое всплытие"](http://hmizgir.livejournal.com/1065.html), Jun. 18th, 2010
