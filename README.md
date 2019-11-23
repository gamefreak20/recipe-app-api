# recipe-app-api
recipe app api source code
    def test_new_user_email_normalized(self):
        email = 'test@TEST.TEST'
        user = get_user_model().objects.create_user(email, 'test123')

        self.assertEqual(user.email, email.lower())
