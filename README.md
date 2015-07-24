smf-helpers
===========

Chef cookbook that installs helper scripts for SMF on Solaris/Illumos
operating systems.

## Usage

```ruby
include_recipe 'smf-helpers::smf-clear'

cron 'clear smf services in maintenance mode' do
  path '/path/to/ruby:$PATH'
  command '/opt/local/bin/smf-clear'
  minute '0,10,20,30,40,50'
end
```
