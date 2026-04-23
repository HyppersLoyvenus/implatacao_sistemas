# TF08 - Relatório da Caça ao Tesouro na AWS

## Aluno
- **Nome:** Antuane Felipe
- **RA:** 3124596

---

## Evidências das Missões

### Missão 1: Explorando Zonas de Disponibilidade

*Screenshot mostrando as Zonas de Disponibilidade de uma região:*

![Evidência Missão 1](Prints/Print_Zonas.PNG)

---

### Missão 2: Grupo "Desenvolvedores" com `PowerUserAccess`

*Screenshot do grupo IAM que criei, com a política de Power User anexada:*

![Evidência Missão 2](Prints/Print_DevGroup.PNG)

---

### Missão 3: O JSON da Política de Administrador

*Este é o `Statement` da política `AdministratorAccess` que concede poder total:*

```json
    "Statement": [
        {
            "Effect": "Allow",
            "Action": "*",
            "Resource": "*"
        }
```

---

### Missão 4: Simulação de Política IAM

*Screenshot do IAM Policy Simulator mostrando que meu usuário `cli-user` **não pode** criar novos usuários (ação `iam:CreateUser` negada):*

![Evidência Missão 4](Prints/Print_PoliciesSimulator.PNG)