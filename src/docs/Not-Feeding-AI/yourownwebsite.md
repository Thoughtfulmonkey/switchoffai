# Your own website

If you host your own website, you can take to try to block AI from using your site's contents as training data.

## Create a robots.txt

A robots.txt file sits in the root directory of your website and provides instructions for software called crawlers. Some crawlers catalogue the internet for search engines. Other crawlers gather training data for generative AI. One of the instructions that you can provide in the robots.txt file is to ask AI crawlers not to steal your content.

!!! note "Note" 
    The instructions in the robots.txt files are only requests. An AI crawler could ignore your request.

To create or update your robots.txt file to try and block AI, complete the following steps:

1. Access the files on your web server. Common methods include the following:
    * If you use hosting with management software, such as CPanel, sign in, and then select the option to access your file server.
    * If you have set up SFTP, open the SFTP client on your computer, and then connect to the server.
    * If you're unsure, contact the person who set up your website.
2. Go to the root of the file directory. This is typically the location where the main `index.html` page for your site is stored.
3. If there is a robots.txt file, choose to edit it. If there isn't a robots.txt file, choose to create one. 

    !!! note "Note" 
        If you use SFTP, you might need to copy the file to your computer, or create it on your computer, before you can edit it.

4. Go to the [ai.robots.txt GitHub repository](https://github.com/ai-robots-txt/ai.robots.txt), and select the [robots.txt](https://github.com/ai-robots-txt/ai.robots.txt/blob/main/robots.txt) file.
5. Copy the contents of the robots.txt file from GitHub to your own robots.txt file.
6. Save your robots.txt. If you edited a copy of the file locally on your computer, copy it back to server.

## Advanced AI crawler blocking

The [ai.robots.txt GitHub repository](https://github.com/ai-robots-txt/ai.robots.txt) includes other methods to block AI crawlers, such as using a .htaccess file to return an error page to AI crawlers. Refer to that repository if you have the technical knowledge to evaluate those methods and implement them.