Bash-script for quick upfloat from the Rails subdirectories to RAILSROOT.
It can be useful to those who constantly live in the console.

# Using

diving example:

`cd app/controllers/admin`

quick surface

`. cdrails`

For convenience possible to make alias, something like:

`alias cdr=cdrails`

And then:

`. cdr`

It is also possible to jump to special Rails-dir:

  `. cdr migrate`

  `. cdr plugins`

  etc.

Ready shortcats:

- models -> app/models' 
- controllers -> app/controllers' 
- helpers -> app/helpers' 
- views -> app/views' 
- layouts -> app/views/layouts'
- migrate -> db/migrate' 
- gems -> vendor/gems' 
- plugins -> vendor/plugins' 

---------------------------------------

For details, see code and `man bash` (about `source`):

> Read and execute commands from filename in the current shell
> environment and return the exit  status  of  the last  command
> executed  from filename.
