
#Loaders

So today I learned about Loaders which allow files to be preprocessed as and when they are required/loaded. 

They provide a powerful way to handle front end build steps.

Loaders are often used to transform files from a different language or to require files. 

Specifying loaders in each module can be repetetive so its best to specify loaders in your Webpack configuration file like follows.



```
{ 
  module: { 
    loaders: [
      // for .jade files 
      {test: /\.jade$/, loader: "jade"},
      // for .css files 
      {test: /\.css$/, loader: "style!css"},
      // for .coffee files
      {test: /\.coffee$/, loader: "coffee-loader"}
    ]
  }
}
          
```
