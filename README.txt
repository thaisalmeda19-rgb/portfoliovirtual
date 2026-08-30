THAÍS DENISY — PORTFÓLIO + ADMIN (FIRESTORE, SEM STORAGE)

ARQUIVOS
- index.html: site público
- admin.html: painel administrativo
- firestore.rules: regras de segurança do Firestore

1) CRIAR O USUÁRIO ADMIN
No Firebase Console:
Authentication > Users > Add user
E-mail: admin@thaisdenisy.app
Senha: Thais202622

A tela do admin pede apenas a senha. O e-mail fica oculto no código para simplificar seu acesso.

2) PUBLICAR AS REGRAS
Firestore > Regras
Apague as regras atuais, cole todo o conteúdo de firestore.rules e clique em Publicar.

3) PUBLICAR O SITE
Suba index.html e admin.html para o mesmo site/Netlify.
Acesse o painel por:
https://SEU-DOMINIO/admin.html

4) COMO AS FOTOS FUNCIONAM SEM STORAGE
O painel redimensiona e comprime as imagens antes do upload.
- capa: aproximadamente até 300 KB
- galeria: aproximadamente até 240 KB por foto
Cada foto da galeria fica em um documento separado do Firestore.

Isso funciona bem para poucas fotos leves.
Não é indicado para galerias grandes, pois o Firestore possui limite de tamanho por documento e cobra por leituras/gravações.

5) MOBILE
As duas páginas foram feitas com layout mobile-first e adaptam para telas pequenas.
