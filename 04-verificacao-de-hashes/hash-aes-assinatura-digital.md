Atividade: Hash, Criptografia AES e Assinatura Digital RSA

Objetivo

Estudar como os algoritmos criptográficos ajudam a proteger evidências digitais, garantindo integridade, confidencialidade e autenticidade.

1. Verificação de hashes

Utilizei os comandos sha256sum -c SHA256SUMS e md5sum -c MD5SUMS para verificar a integridade dos arquivos.

Resultado: três arquivos foram verificados corretamente, mas relatorio_financeiro.csv apresentou divergência nos dois testes.

2. Criptografia AES-256

Compactei as evidências e usei o OpenSSL para criptografar o pacote com AES-256-CBC. Testei a descriptografia com uma senha incorreta e depois com a senha correta.

Resultado: a senha incorreta não permitiu recuperar o pacote. Com a senha correta, os hashes SHA-256 do pacote original e do recuperado foram iguais.

3. Assinatura digital RSA

Gerei um par de chaves RSA, criei um laudo e assinei seu conteúdo com a chave privada. Em seguida, verifiquei a assinatura usando a chave pública.

Resultado: a assinatura original foi validada com Verified OK. Depois de alterar o laudo, a verificação apresentou Verification failure.

Conclusão

A atividade demonstrou como o hash ajuda a verificar a integridade, o AES protege a confidencialidade e a assinatura digital RSA permite verificar a autenticidade e detectar alterações no documento assinado.

Segurança: as chaves privadas, senhas e arquivos temporários não devem ser publicados no repositório.
