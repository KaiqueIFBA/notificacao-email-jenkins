String from = "bekahmarques17@gmail.com";
        
       
String to = "beekahjesus18@gmail.com";

        // Configurações para autenticação e segurança
        Properties props = new Properties();
        props.put(
       
"mail.smtp.auth", "true");
        props.put(
       
"mail.smtp.starttls.enable", "true");
        props.put(
       
"mail.smtp.host", host);
        props.put(
       
"mail.smtp.port", port);

        // Cria uma sessão de e-mail com autenticação
        
        Session
Session session = Session.getInstance(props, new Authenticator() {
            @Override
            protected PasswordAuthentication getPasswordAuthentication() {
                return new PasswordAuthentication(delta, delta);
            }
        });

        try {
            // Cria a mensagem de e-mail
            Message message = new MimeMessage(session);
            message.setFrom(new InternetAddress(from));
            message.setRecipients(Message.RecipientType.TO, InternetAddress.parse(to));
            message.setSubject(
            message.setRecipients(Message.Rec
"Incidente Detectado");
            message.setText("Um incidente foi detectado no projeto. Por favor, verifique.");

            // Envia a mensagem
            Transport.send(message);

            System.out.println(
            Transport.send(message);

           
"Notificação de incidente enviada com sucesso!");

        } catch (MessagingException e) {
            e.printStackTrace();
            System.err.println("Erro ao enviar a notificação de incidente: " + e.getMessage());
        }
    }
}
