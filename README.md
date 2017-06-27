## n

n is a simple rails scaffold script for generating a model and all it's CRUD/L features without the mass of unnecessary information usually produced with rails' built-in scaffolding.

#### Usage
* From inside the root of your rails project, run `$ git clone https://github.com/seanpierce/n`
* When you're ready to scaffold your model, run `$ ./n/model`
* Follow the script's prompts
* in your **config/routes.rb** file, add "resources :_plural-lowercase-model-name_"

```
Rails.application.routes.draw do
    resources :animals
end
```

#### Notes
This script will generate the following files and directories, and will also include corresponding code in each file to get you started.
* app/controllers/**classname**\_controller.rb
* app/models/**classname**.rb
* app/views/**classname**/\_form.html.erb
* app/views/**classname**/edit.html.erb
* app/views/**classname**/index.html.erb
* app/views/**classname**/new.html.erb
* app/views/**classname**/show.html.erb
* spec/models/**classname**\_spec.rb


#### Authors
Sean Pierce, Tyler Stephenson
#### License
MIT &copy; 2017
