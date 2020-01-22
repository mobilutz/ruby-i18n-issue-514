Example Rails App for https://github.com/ruby-i18n/i18n/issues/514


Run:
```
> bundle install
> rails c

irb> I18n.t('activerecord.models.model', count: 1)

irb> I18n.t('activerecord.models.broken_model', count: 1)
{:one=>"My Model Translation", :other=>"My Models Translation", :some_other_key=>{:key=>"Value"}}
```

See locales in https://github.com/mobilutz/ruby-i18n-issue-514/blob/master/config/locales/en.yml


INFO:

Problem solved with adding `rails-i18n` gem!
