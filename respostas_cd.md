# Respostas da Atividade — Entrega Contínua (CD) com GitHub Actions

## 🧠 Perguntas rápidas

**1. O que é CD e qual sua relação com CI?**  
**Resposta:**  
CD (Continuous Delivery/Deployment) é a prática de automatizar a entrega ou publicação de uma aplicação após os testes passarem. Ele complementa o CI (Continuous Integration), que garante que o código seja constantemente testado e validado a cada push. Ou seja, CI valida o código, CD entrega ele.

**2. Quais são os benefícios da entrega contínua?**  
**Resposta:**  
- Publicações mais rápidas e frequentes.  
- Redução de erros humanos na implantação.  
- Maior confiança no código e no processo de deploy.  
- Feedback rápido para o time de desenvolvimento.  

**3. Qual é a principal diferença prática entre CI e CD?**  
**Resposta:**  
CI foca em testar e validar o código automaticamente, enquanto CD foca em entregar/deployar esse código automaticamente após passar nos testes.

**4. O que aconteceria se o teste falhasse antes do deploy?**  
**Resposta:**  
O deploy não seria executado, evitando que código com erro seja publicado. Isso protege a estabilidade da aplicação.

**5. Como a entrega contínua aumenta a confiança do time no processo?**  
**Resposta:**  
Porque garante que todo código validado passa por testes automáticos e, somente se estiver correto, é publicado. Isso reduz riscos e retrabalho.

---

## 💻 Mão na Massa

### Etapa 1 – Criar arquivo simples de página web
```bash
echo "<h1>Aplicação implantada via GitHub Actions</h1>" > index.html
git add index.html
git commit -m "Adiciona página inicial"
git push origin main
