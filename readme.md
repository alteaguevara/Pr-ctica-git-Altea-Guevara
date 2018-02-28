# Práctica GIT

### Guevara Alonso, Altea

--

**1. ¿Qué comando utilizaste en el paso 11? ¿Por qué?**

`git reset --hard HEAD~1` 

Este comando deshace el último commit y además lo que hay en el working copy.

--

**2. ¿Qué comando utilizaste en el paso 12? ¿Por qué?**

`git reset fa0865e` 

Para rehacer el paso anterior (que consistía en deshacer un commit), miré el número identificador del commit que quería recuperar con el comando `git reflog`. Utilicé `git reset` para volver a él.
--

**3. El merge del paso 13, ¿Causó algún conflicto?¿Por qué?**

Hice `git merge master`. La consola me decía `Already up to date` porque en la rama master por su cuenta no había realizado ningún cambio. Styled ya contenía el commit inicial de master, pues deriva de él. 
--

**4. El merge del paso 19, ¿Causó algún conflicto?¿Por qué?**

No me ha causado ningún conflicto, me notificó que `merge made by the ‘recursive’ strategy`.  A continuación utilicé el comando `git branch --merged` y `git branch --no-merged` para comprobar que la unión de ramas fue exitosa ya. Ninguna de las ramas contenía a la otra previamente, pues ambias fueron creadas desde master. 

--

**5. El merge del paso 21, ¿Causó algún conflicto?¿Por qué?**

No parece haber causado ningún conflicto. 

--

**6. ¿Qué comando o comandos utilizaste en el paso 25?**

`git log --graph` 

--

**7. El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**

Sí. Al derivar title de master y no haber realizado más cambios en master, no era una estructura ‘tipo árbol’, es decir, no había realmente varias ramas. Al juntar ambas, sería como desplazar o incluir title en master de forma simple sin necesidad de hacer un nuevo commit.



--

**8. ¿Qué comando o comandos utilizaste en el paso 27?**

`git reset HEAD~1`

--

**9. ¿Qué comando o comandos utilizaste en el paso 28?**

`git reset --hard HEAD~1` 

--

**10. ¿Qué comando o comandos utilizaste en el paso 29?**

`git branch -D title` 

--

**11. ¿Qué comando o comandos utilizaste en el paso 30?**

Introducimos `git reflog`para ver TODOS los commits, incluso los que ya no salen en `git log` porque los hemos deshecho. Después copiamos el identificador del merge e introducimos `git reset 45b7097`.

--

**12. ¿Qué comando o comandos usaste en el paso 32?**

Introducimos `git log` para ver el identificador del primer commit, e  introducimos `git reset 8592710`.

--

**13. ¿Qué comando o comandos usaste en el punto 33?**

Introducimos `git reflog`para ver TODOS los commits, incluso los que ya no salen en `git log` porque los hemos deshecho. Después copiamos el identificador último commit que hicimos e introducimos `git reset 6e0dbcc`.




