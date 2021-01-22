# Conclusion

That's all there is to deploying multiple instances of your CodeIgniter application.

Now, you only need to update once and all your deployed instances will use that updated file. This reduces code redundancy and makes maintenance extremely easy.

In this guide, we have used sub-domains as our deployment points but there is no hard and fast rule that requires you to do this. You may deploy the individual instances in normal directories.
However, you will want to remove the domain filter from your ``.htaccess`` and update your ``base_url`` accordingly.

Thank you for reading!
