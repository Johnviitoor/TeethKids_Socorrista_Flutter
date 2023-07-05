# App de Emergência Dentária

Este é um aplicativo Flutter desenvolvido no Android Studio que permite aos usuários solicitar assistência odontológica de emergência direta para o dentista. O aplicativo também comunica-se com um app em kotlin do dentista/clínica odontológica.

## Recursos

- Solicitar assistência odontológica de emergência
- Marcar a localização do usuário ou  dentista com base em 3 endereços cadastrados pelo usuario
- Fazer uma ligação com base no numero de telefone cadastrado do usuario/dentista
- Visualizar o endereço no mapa cadastrados usuario/dentista

## Instalação

1. Clone o repositório: `git clone https://github.com/seu-link-do-repositorio`
2. Abra o projeto no Android Studio.
3. Instale as dependências necessárias executando o seguinte comando no terminal:
   ```
   flutter pub get
   ```

## Uso

1. Conecte seu dispositivo Android ou configure um emulador.
2. Execute o aplicativo usando o seguinte comando no terminal:
   ```
   flutter run
   ```
3. Conceda as permissões necessárias para o aplicativo acessar a localização do dispositivo e fazer chamadas telefônicas.
4. Na tela inicial do aplicativo, toque no botão "Emergência" para solicitar assistência odontológica.
5. O aplicativo marcará automaticamente sua localização atual no mapa.
6. Após enviar a solicitação de emergência, o aplicativo fornecerá a opção de ligar diretamente para o dentista.
7. Toque no botão "Ligar" para iniciar a chamada.

## Configuração

Para configurar o aplicativo com a clínica odontológica e o serviço de mapas de sua preferência, siga estas etapas:

1. Abra o projeto no Android Studio.
2. Navegue pelos arquivos de código relevantes:
   - Contato do dentista: `lib/screens/emergency_screen.dart`
   - Integração do mapa: `lib/screens/emergency_screen.dart`
3. Modifique as informações de contato do dentista, como número de telefone e endereço de e-mail, na seção de código correspondente.
4. Personalize a integração do mapa substituindo o endereço padrão pelo endereço da clínica odontológica desejada.

```dart
// Informações de Contato do Dentista (emergency_screen.dart)
final String dentistPhoneNumber = '1234567890';
final String dentistEmail = 'dentista@exemplo.com';

// Integração do Mapa (emergency_screen.dart)
final String dentalClinicAddress = 'Rua Odontológica, 123, Cidade, País';
```

## Contribuição

Contribuições são bem-vindas! Se você encontrar algum problema ou tiver sugestões de melhoria, por favor, envie uma issue no repositório do GitHub.

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).
