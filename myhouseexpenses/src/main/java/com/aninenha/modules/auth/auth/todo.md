# registro - fluxo

Client <br>
  │ <br>
POST /auth/register <br>
  │<br>
AuthController <br>
  │<br>
AuthService<br>
  │<br>
UserService<br>
  │<br>
UserRepository<br>
  │<br>
PostgreSQL

> usuário criado <br>
> senha criptografada

# Login - fluxo

Client
<br>  │
<br>POST /auth/login
<br>  │
<br>AuthController
<br>  │
<br>AuthService
<br>  │
<br>Spring Security AuthenticationManager
<br>  │
<br>UserDetailsService
<br>  │
<br>UserRepository

>token JWT

# Endpoint segurança

GET /users/me <br>

Client envia JWT
<br>↓
<br>Spring Security Filter
<br>↓
<br>Token validado
<br>↓
<br>SecurityContext preenchido
<br>↓
<br>Controller executa

>>> Pastas vazias adicionar um .gitkeep