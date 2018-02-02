OpenAPI
==========

The original (https://github.com/ant31/openapi - the basis of the current Ruby Gem @ rubygems.org) was somewhat buggy, and had not been updated for several years, so I forked it and fixed at least some of the bugs - enough to make it do what I needed it to do!

I do not promise that all bugs are fixed.

Good luck!




# Examples



    require 'openapi'
    
    api = OpenAPI::Client.new(:site => "http://petstore.swagger.io/v2/", :request_timeout => 60 )
    
    response = api.do_request('get', 'pet/1', params: {}, body: nil, headers: {}, options: {:skip_auth => true})
    
    puts response

