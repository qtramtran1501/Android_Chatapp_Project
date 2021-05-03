# Android_Chatapp_Project

//Fix lỗi logout
        MainActivity:
  115. mAuth.signout(); ->  FirebaseAuth.getInstance().signOut();
  116. finish();       -> startActivity(new Intent(MainActivity.this, LoginActivity.class));
  117. return true;    -> finish();
