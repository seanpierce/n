## n

n is a simple rails scaffold script for generating a model and all it's CRUD/L features without the mass of unnecessary information usually produced with rails' built-in scaffolding.

#### Usage
* From inside the root of your rails project, run `$ git clone https://github.com/seanpierce/n`
* When you're ready to scaffold your model, run `$ ./n/model`
* Provide the script with the singular and plural versions of your intended class name.

#### Notes
This script will:
* generate the following files
  * app/controllers/**classname**\_controller.rb
  * app/models/**classname**.rb
  * app/views/**classname**/\_form.html.erb
  * app/views/**classname**/edit.html.erb
  * app/views/**classname**/index.html.erb
  * app/views/**classname**/new.html.erb
  * app/views/**classname**/show.html.erb
  * spec/models/**classname**\_spec.rb (if applicable)
* write starter code to each file  

The script will **not**
* create class associations (you can start this process by nesting your resources in config/routes, then write your associations into your app/models files)
* predict class attributes

At the bottom of each class controller, the script declared placeholder values as strict parameters. These will need to be changed for your class to be successfully implemented. Example:
```ruby

private
  def classname_params
    # Use strict parameters, replace placeholder info below with your class' actual attributes
    params.require(:classname).permit(:attribute1, :attribute2, :attribute3)
  end
end
```
Simply change attribute1-3 to reflect your class' properties.

#### Bugs/ Issues
No known bugs. If a bug is discovered please create an <a href="https://github.com/seanpierce/n/issues/new">issue</a>. Pull requests always welcome, too.

#### Authors
Sean Pierce, Tyler Stephenson
#### License
MIT &copy; 2017
