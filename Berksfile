source "https://supermarket.chef.io"

#cookbook 'logstash', :git => 'https://github.com/PaytmLabs/chef-logstash.git', :ref => 'feature-fix-java-opts'
cookbook 'puncha-kibana', :git => 'https://github.com/PaytmLabs/chef-puncha-kibana.git', :ref => 'feature-small-fixes'
cookbook 'elasticsearch2', :git => 'https://github.com/PaytmLabs/chef-elasticsearch.git', :ref => 'es2-namespace'

## Due to a design decision in berkshelf to not recursively resolve dependencies, we must declare all dependencies of our dependencies, to the full depth of the recursion

# Dependencies of masala_ldap:
cookbook 'openldap', :git => 'https://github.com/PaytmLabs/chef-openldap.git', :ref => 'feature-our-fixes'
cookbook 'masala_ldap', :git => 'https://github.com/PaytmLabs/masala_ldap.git', :ref => 'develop'

# Dependencies of masala_base:
cookbook 'ixgbevf', :git => 'https://github.com/PaytmLabs/chef-ixgbevf.git', :ref => 'master'
cookbook 'system', :git => 'https://github.com/PaytmLabs/chef-system.git', :ref => 'feature-fix-debian-tz'
cookbook 'masala_base', :git => 'https://github.com/PaytmLabs/masala_base.git', :ref => 'develop'

## Now load the primary metadata
metadata
