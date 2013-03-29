You need to create a Facebook app and insert http://localhost:3000 as the website

    config.omniauth :facebook, "APP_ID", "APP_SECRET", {:scope => 'publish_stream,offline_access,email,read_stream,read_friendlists,user_photos,friends_photos,manage_friendlists'}


* environments/development.rb

change the mailing method and credentials

    config.action_mailer.smtp_settings = {
      :enable_starttls_auto => true,
      :address => "smtp.gmail.com",
      :port => 587,
      :domain => "gmail.com",
      :authentication => :login,
      :user_name => "your-email",
      :password => "your-password",
    }


