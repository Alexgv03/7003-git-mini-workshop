# Git Mini Workshop

¡Bienvenido al taller de Git! En esta tarea práctica aprenderás a hacer **fork**, trabajar con **feature branches**, seguir los éstandares de **commit**, resolver **merge conflicts** y abrir un **Pull Request (PR)**.

Para proteger tus datos personales en este repositorio público, **no escribas tu nombre real ni tu ID de estudiante en ningún archivo**. Utilizarás un hash anónimo generado por un script local de Python.

---

## 🛠️ Prerequisitos

Asegúrate de tener instaladas las siguientes herramientas en tu máquina local:

* [Git](https://git-scm.com/)
* [Python 3.x](https://www.python.org/)
* Un editor de código (por ejemplo, VS Code, Neovim, Emacs)

---

## 🛠️ Ejercicios del Workshop

### Ejercicio 1: Basicos de Git
*(Sigue las intrucciones de abajo sobre la rama `main`)*

---

### Ejercicio 2: Práctica de rebases interactivos

Este ejercicio se encuentra en su propia rama dedicada.

#### Instrucciones:
1. **Fetch y checkout en la rama del ejercicio:**
   ```bash
   git fetch origin
   git checkout exercise/rebase-practice
   ```

---

# 🔀 Ejercicio de rebases interactivos

En este ejercicio, tendrán que limpiar el historial de commits de ésta rama usando `git rebase -i`.

## 📋 Instrucciones

Cada commit en esta rama contiene instrucciones específicas en sus **commit message**, indicando qué acción tienen que realizar (ej., *squash*, *reword*, *edit*, *drop*, o *amend*).

### Intrucciones paso a paso

1. **Revisa el historial de commits**
   Ejecuta la siguiente instruccion para ver la lista de commits y sus instrucciones:
   ```bash
   git log --oneline
   ```
2. **Inicia un rebase interactivo**
   Empieza el rebase interactivo desde el commit donde todo inició:
   ```bash
   git rebase -i <base_commit_hash>
   ```
3. Realiza las tareas solicitadas
4. Pushea tu rama modificada en:
   ```bash
   git push -u origin exercise/<username>-rebase
   ``


Tip: Si en algún momento cometes algún error durante el rebase, para abortar usa este comando:

```bash
git rebase --abort
```