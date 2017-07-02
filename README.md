# blog.js-password-reset

make sure to add these fields to the user model:

    email: {type: String, unique: true, required: true},
    resetPasswordToken: String,
    resetPasswordExpires: Date,
