var nodemailer = require('nodemailer');

var transporter = nodemailer.createTransport({
    host: "smtp.gmail.com", // hostname
    secure: false, // use SSL
    port: 465, // port for secure SMTP
    auth: {
        user: "",
        pass: ""
    },
    tls: {
        rejectUnauthorized: false
    }
});




var mailOptions = {
    from: 'tywoplenty@gmail.com',
    to: 'tywotaiwo@gmail.com',
    subject: 'Sending Email using Node.js',
    text: 'That was easy!'
};

transporter.sendMail(mailOptions, function(error, info){
    if (error) {
        console.log(error);
    } else {
        console.log('Email sent: ' + info.response);
    }
});