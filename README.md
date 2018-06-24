# Webpack-3-4-Bootstrap-3-4
Webpack 3 &amp; 4 with Bootstrap 3 &amp; 4

Thou we are only using Webpack 4 in this tutorial we have tried to use Webpack 3 and it works perfectly fine.

To do so, you need to use yarn to add two different versions of the bootstrap dependency.

<p>// add the latest version of bootstrap Currently 4.1.1</p>
<p>yarn add bootstrap@latest</p>
<p>// add a legacy version of bootstrap 3.3.7 under and different name</p>
<p>yarn add bootstrap3@npm:bootstrap@3.3.7</p>

In webpack.config.js, 

Your entry must be the object instance and have two different entry points otherwise the two versions will conflict, 

  entry: {
    bootstrap4: './src/bootstrap4.js',
    bootstrap3: './src/bootstrap3.js'
  },
  
