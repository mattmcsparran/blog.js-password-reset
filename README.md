# blog.js-password-reset

make sure to add these fields to the user model:

    email: {type: String, unique: true, required: true},
    resetPasswordToken: String,
    resetPasswordExpires: Date,


also make sure you have added the dependencies to the route or the app:

            var async = require("async");
            var nodemailer = require("nodemailer");
            var crypto = require("crypto");
