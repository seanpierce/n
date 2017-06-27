## n

n is a simple rails scaffold script for generating a model and all it's CRUD/L features without the mass of unnecessary information usually produced with rails' built-in scaffolding.

#### Usage
* From inside the root of your rails project, run `$ git clone https://github.com/seanpierce/n`
* When you're ready to scaffold your model, run `$ ./n/model`
* Follow the script's prompts
* in your **config/routes.rb** file, add "resources :_plural-lowercase-model-name_"
  * ex:
  ```
  Rails.application.routes.draw do
      resources :animals
  end    
  ```

#### Authors
Sean Pierce, Tyler Stephenson
