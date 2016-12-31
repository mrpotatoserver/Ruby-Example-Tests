# Ruby Example Tests
[//]: # "[![Travis Status](https://travis-ci.org/saucelabs-sample-test-frameworks/Ruby-RSpec-Selenium.svg?branch=master)](https://travis-ci.org/saucelabs-sample-test-frameworks/Ruby-RSpec-Selenium)"

## Important Disclaimer
This code is provided on an "AS-IS” basis without warranty of any kind, either express or implied, 
including without limitation any implied warranties of condition, uninterrupted use, merchantability, 
fitness for a particular purpose, or non-infringement. 
Your tests and testing environments may require you to modify this framework. 
Issues regarding this framework should be submitted through GitHub. 
For questions regarding Sauce Labs integration, please see the [Sauce Labs documentation](https://wiki.saucelabs.com/). 
This framework is not maintained by Sauce Labs Support.


## Purpose
Use this project only if you have experience setting up frameworks in Ruby, ideally these examples
 would be incorporated in an existing project you would like to adapt to run on Sauce Labs.

If you do not have an existing project and would like to use Ruby, it is recommended to look at the 
 [Watir Examples](http://www.notimplementedyet.com). If this is specifically for a Rails project
 and the developers who will be creating and implementing the new project have experience with
 Capybara, it is recommended to look at the [Capybara Examples](http://www.notimplementedyet.com)
 
 
## Technologies demonstrated in this project:

#### RSpec
1. [Pass Information to Saucelabs](https://github.com/titusfortner/Ruby-Selenium-Examples/blob/master/spec/spec_helper.rb#L8-L30)
2. [Execute Tests in Parallel](https://github.com/titusfortner/Ruby-Selenium-Examples/blob/master/Rakefile#L26)
3. [Integrate with Applitools](https://github.com/titusfortner/Ruby-Selenium-Examples/blob/master/spec/spec_helper.rb#L32-L36)

### Cucumber
1. [Pass Information to Saucelabs](https://github.com/titusfortner/Ruby-Selenium-Examples/blob/master/features/support/env.rb#L7-L31)
2. [Execute Tests in Parallel](https://github.com/titusfortner/Ruby-Selenium-Examples/blob/master/Rakefile#L35)
3. [Integrate with Applitools](https://github.com/titusfortner/Ruby-Selenium-Examples/blob/master/features/support/env.rb#L33-L37)


### Appium for iOS
1. [Spec Examples](https://github.com/titusfortner/Ruby-Selenium-Examples/tree/master/spec/ios)
2. [Feature Examples](https://github.com/titusfortner/Ruby-Selenium-Examples/tree/master/features/step_definitions)
3. [Parameter Examples](https://github.com/titusfortner/Ruby-Selenium-Examples/blob/master/Rakefile#L107-L112)

### Appium for Android
1. [Spec Examples](https://github.com/titusfortner/Ruby-Selenium-Examples/tree/master/spec/android)
2. [Feature Examples](https://github.com/titusfortner/Ruby-Selenium-Examples/tree/master/features/step_definitions)
3. [Parameter Examples](https://github.com/titusfortner/Ruby-Selenium-Examples/blob/master/Rakefile#L148-L153)

### Selenium for Desktop Browsers
1. [Spec Examples](https://github.com/titusfortner/Ruby-Selenium-Examples/tree/master/spec/desktop)
2. [Feature Examples](https://github.com/titusfortner/Ruby-Selenium-Examples/tree/master/features/step_definitions)
3. [Parameter Examples](https://github.com/titusfortner/Ruby-Selenium-Examples/blob/master/Rakefile#L86-L89)


## Requirements to Run These Examples (OSX/MacOS)

1. Global Dependencies
    * [Install Ruby](https://www.ruby-lang.org/en/documentation/installation/)
    * Or Install Ruby with [Homebrew](http://brew.sh/)
    ```
    $ brew install ruby
    ```
    * Install [Rake](http://docs.seattlerb.org/rake/)
    ```
    $ gem install rake
    ```
    * Install bundler (Sudo may be necessary)
    ```
    $ gem install bundler
    ```

2. Sauce Credentials
    * In the terminal export your Sauce Labs Credentials as environmental variables:
    ```
    $ export SAUCE_USERNAME=<your Sauce Labs username>
	$ export SAUCE_ACCESS_KEY=<your Sauce Labs access key>
    ```

3. Project Dependencies
	* Install packages (Use sudo if necessary)
	```
	$ bundle install
	```
    * Set Build ID (Optional)
    ```
    $ export BUILD_TAG=sauce_automated_build_name
    ```


## Running Tests

1. Run RSpec specs on Sauce in Parallel:
	```
	$ bundle exec rake test_rspec
	```

2. Run Cucumber Features on Sauce in Parallel:
	```
	$ bundle exec rake test_cucumber
	```

3. Execute Tests on Sauce in Parallel using an environment variable:
	```
	$ TEST_RUNNER=rspec bundle exec rake
	```

View the results on your [Sauce Labs Dashboard](https://saucelabs.com/beta/dashboard/)


### Contributing

This project is open source! 
The maintainers welcome the community to [submit an issue](http://notimplementedyet.com/issues#new) with ideas or bug reports, 
and [making pull requests](http://notimplementedyet.com/pulls#new) with bug fixes and suggested code improvements


## License

This project is available under the terms of the [MIT License](http://opensource.org/licenses/MIT).


## Additional Resources
##### [Sauce Labs Documentation](https://wiki.saucelabs.com/)

##### [SeleniumHQ Documentation](http://www.seleniumhq.org/docs/)

##### [Appium Documentation](https://appium.io/documentation.html/)

##### [RSpec Documentation](http://rspec.info/documentation/)

##### [Cucumber Documentation](https://cucumber.io/docs/)

##### [Applitools Documentation](https://applitools.com/resources/#Documentation/)

##### [Ruby Documentation](http://ruby-doc.org/)

##### [Stack Overflow](http://stackoverflow.com/)
* A great resource to search for issues not explicitly covered by documentation.
