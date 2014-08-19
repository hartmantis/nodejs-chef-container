Node.js Docker Image
====================

A Docker image with Node.js installed, built using Chef-Container.

Requirements
============

Obviously, Docker is required. This image build utilizes
[Chef](https://getchef.com) and
[Knife-Container](https://github.com/opscode/knife-container) to construct the
image using Chef.

Usage
=====

Clone this project into a `dockerfiles/roboticcheese` directory (this is
important, as knife-container currently expects a specific directory structure).

Install the dependent gems using the ChefDK or another Ruby environment:

    (chef exec) bundle install

Run the build:

    (chef exec) bundle exec knife container docker build roboticcheese/nodejs -d ../..

Contributing
============

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Run style checks and RSpec tests (`bundle exec rake`)
4. Commit your changes (`git commit -am 'Add some feature'`)
5. Push to the branch (`git push origin my-new-feature`)
6. Create new Pull Request

License & Authors
=================
- Author: Jonathan Hartman <j@p4nt5.com>

Copyright 2014, Jonathan Hartman

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
