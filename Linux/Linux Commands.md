---
tags:
---
```
uname -a
```
![[Pasted image 20250108145237.png]]

```
head -n 1/etc/issue
```
```
mount
```
```
date
```
```
uptime
```
```
whoami
```
```
man bash 
```
```
env
```
```
echo $NAME
```
```
export a='anand'
```
```
echo $a
```
```
$PATH
```
```
$HOME
```
```
echo $SHELL 
```

Redirections
```
> [[read]] input  commands from the file
```
```
< # write output commands to file
```
```
>/dev/null [[discard]] output command
```
```
/dev/null [[Blackhole]] [[bit]] bucket
```
```
>> file # append output to file
```
```
command 1|commands 2# pipe output of commands 1 to commands2
```
Directory Operations
```
pwd [[print]] working dire
```
make directory dir
```
mkdir anand
```
change dir
```
cd anand
```
go up a previous dir
```
cd..
```
list file and dir
```
ls
```
ls options
```
ls -a
```
```
ls -R
```
```
ls -r
```
```
ls -t
```
```
ls -S
```
```
ls -l
```
```
ls -1
```
```
ls -m
```
```
ls -Q
```
```
ls -lrt
```
Search files
```
grep --help
```
```
grep *.txt
```
```
grep -i 'echo' a.txt
```
```
grep -r age.txt
```
```
find /mnt/d/wsl/devops/ext4.vhdx *.txt
```
```
find /mnt/d/wsl/*/ext4.vhdx *.txt
```
```
whereis bash
```
```
locate /mnt/c/Users/Dell/Downloads/*.log
```
![[Pasted image 20250108161958.png]]
![[Pasted image 20250108162253.png]]

File Operations
```
touch 1.txt 2.log 3.py
```
```
cat 1.txt 2.log 3.py
```
```
less 1.txt 2.log 3.py
```
```
file 1.txt 2.log 3.py
```
```
cp 1.txt 2.txt
```
```
mv 1.txt 2.txt
```
```
rm 1.txt
```
```
rm -rf 1.txt
```
```
head age.txt
```
```
head -n age.txt
```
```
tail -n age.txt
```
Process Management
```
ps
```
```
top
```
```
kill pid
```
```
pkill python3
```
```
killall python3
```
```
kill -9 <pid>
```
```
killall
```

File Permissions
```
chmod 777 file
```
Link file
```
ln a.txt hardlink.txt
```
![[Pasted image 20250108145237.png]]

```
ln -s c.txt d.txt
```


![[Pasted image 20250108145317.png]]

```
touch file.txt file1.txt a.py b.py
``````

``````
touch -d "2002-01-31 15:45:30" anand.txt
``````
![[Pasted image 20250108163719.png]]

``````
touch -m -t 200201311530.45 a.txt
``````
![[Pasted image 20250108163805.png]]

```
touch {1..2}.py
``````

``````
touch {1..1000}.txt
``````

``````
touch {A..Z}.txt
``````

``````
touch {a..z}.py
``````

``````
stat anand.txt
``````
![[Pasted image 20250108163915.png]]

```
ln -s c.txt d.txt
```
![[Screenshot 2024-12-26 142604.png]]


![[Screenshot 2024-12-26 190730.png]]

![[Pasted image 20250108213317.png]]
![[Pasted image 20250108213335.png]]
![[Pasted image 20250108213346.png]]
![[Pasted image 20250108213354.png]]
![[Pasted image 20250108213401.png]]
![[Pasted image 20250108213409.png]]
![[Pasted image 20250108213502.png]]
![](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAA0QAAACNCAYAAACXFrrPAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsMAAA7DAcdvqGQAADh+SURBVHhe7d19dBRVnjfwb3c6IWlIIAm9MYEmCoSGZJIeEYHsxEMcViZRcHhWwBkdBdnjg0cYVHjmAD7MHHZkITw7sjqKIzsPgjo7L8AZZIc1WRyX5Bk5QAbFhoUQXoXwYgwEIdJpkqb7+ePWra6q7nRXoIPE/n7O6RO66vate29VQv36vpSlX79+QRgsWrQIlZWVqKqqQk1NjW5fRUUFFi9ejOrqaqxatQq1tbWorq6Gx+NRt2v/vWrVKvWzy5YtQ3l5OcrLy3V5QnPMaPsilacnrF27FgAwZ84c4y44HA48+uijKC4uVre5XC40NjZGTB+tXohxrNraWuMmVVVVFQB0u52jidXOtbW1YfWM9ZmuxPpcd+se6TqU22OV2eFwYNOmTdi9ezcWL16M0tJSrFy5Eps3b8brr78OmChPpDrcKDPX2Nq1a+FyuXTn2HitxSMf4++71NU1Nm/ePEybNg1LlizBrl27dPtupUjnHQDeffddeL3esO3Gtou0r6vzbObaeP/999HU1BR2XCMzxzLWK9JnIm3TGjVqFH71q1+htrYWy5YtA5S85e+AWbGuH8SxzGbEOhcw+XcjUr2g5K/9XYhV5ni1MxER9SyrcQNFt3r1ajz44IM4f/48Tpw4gRMnThiTxJXH40FVVVXY6+OPPzYmvWlXr141bvpa3aq6t7S0wOPxoKSkBADwve99DwDw4Ycf6tLdqvLE6xqLVz7dMWHCBDQ2Nn6twVBXHA4HnE4nfD6fcddNi9e1cat+BxsaGuDxeDB27FgAwIwZMwAAn3zyiSHlrROvusfrXJgRq8y3YzsTEVG4HgmITp06BQDIy8vTbS8qKtK97wmlpaVwOBzGzXFRUVEBp9OJDRs2YNmyZVi1ahXeeustY7Juc7lcxk0AgKamJhQUFODjjz9GTU2N7tXS0hL3dj527BgQIT+psbERLpcLo0aNUrcNHToU0JzzeIlVd7PMltnj8cBut2PGjBkoKiqCx+NBQ0ODuj9e5YklXtdYvPLpzjU2e/ZsOByOsEDyRsX7d3nhwoWAcq7jycy1cfToUbhcLpSWlho/rnMrfwd37twJu92O2bNnY/To0fB6vdi4caMx2U0zW+ZYdTfDzLnojoqKCvXfMpjRMlPmW9XORER045JSUlJEP77yx/+RRx7B0KFDMXDgQNhsNtxzzz1obW3FhQsXAADDhw9HWVkZjh07hp07d2LWrFk4duwYmpub1e3vvfceSktLUVRUhLvvvhtutxtPPvkk0tLS0LdvX2zYsAFQbqAmTZqEsrIy9Zg5OTkoKytDeno6hg8fHrM8WrNnz8bChQvhcrlQE2H4gllTpkwBAGzbtk23PTk5GZMnT0ZGRgb8fj9Gjx6N+fPn48qVK0hPT0dOTg7q6+tj1kv+JwoAY8aMwZ133qm215QpU3D16lWcOXMG7e3tuP/++zF58mQUFxfjnnvuQVlZGR544AHU1tbiwoULptrZrMuXL2Py5MkoLCxEQUEBxo0bh7KyMgQCAZw5cwZ2ux333nsvxo0bh6FDh6rBQ2NjI9avX2/MLiIz1xiAmHU3cx3KGxEzZd63bx9mzJgBp9OJ3NxcbN++Hfv27TNdnngxe41NmTIFAwcO1J3jsrIyFBQUYMOGDXHLpzvX2IIFC9DR0aEODboZN/u7PGvWLASDQQwdOhRlZWV4/vnn4XK54PF4sHLlSiCOf3/MXBuXL1/G3/7t36KyshIjR45U00yZMgV//vOf1bxu9nfQ7O8XABw8eBAPPfQQsrOzMWjQIBw+fFhXFjNiXT8AYpZZilV3M2KdC7N/N2S98vPz4Xa7UV5ejoceegjJyclYvXq12pZmyhyPdiYiop6l6yFyu92orKxUeyzGjx+PyspK5Ofna5OZsnTpUng8HjXP8+fPY+/evbo048aNQ2Vlpe6Y8r3b7e52ec6dOwev14tLly4Zd8VFQ0MD3nnnHWRlZWHx4sWYPn06duzYgdbWVjgcDkybNg0wUS+tNWvWwOPxwOVyobKyEsOGDUP//v0BADU1NaiqqsLRo0fVuldWViI1NVX9vJl2NqulpQW//OUvcfHiRZSXl6vHkzZu3Ig33ngDUOpTUFCA3bt3Y+nSpZpcojN7Ts3U3YzulHn//v1wOp3wer1hvSnxKk8sZq+xWOKVD0xeY7JHqrq6Wrf9RsXjd9nhcKjnyefzYfPmzXjuuefU/bF+T+N5re7atQsvvfSSOjRTphk2bJgur5v9HTRbZmnv3r1wuVxwOBw4cuSIcXdcxCqzFKvuZpg5F92xY8cOFBUVoby8HFevXsUbb7yh6zk2W+Zb0c5ERHTjLJEWVSAi6o5XX30VBQUFmDlz5g0NTaKvT1VVFUpKSnjuNLpaVOFmsJ2JiG5fPTKHiIgSy7lz57Bhwwbe6PUys2fPxvjx41FXV8dz14PYzkREtzf2EBERJZCKigqUl5dj0KBBcDqdaGpqwhNPPGFMltDi0UPEdiYi6j3YQ0RElEDcbjdKSkrg9XqxefNm3qT3ELYzEVHvwR4iIiIiIiJKWOwhIiIiIiKihKV7DhERfT3yJ61HanYhrp79yLiLTGIb3pi1a9fC7/frno9GdCMWLVqEQYMG4eDBg8Zd1EvbpzeW2Yxvar3MSOS6R2OqhyhlAWDfbtz69bndykN0M3LGLsGAEdOQlJJu3NUrOdxz4fzua8bNPao3tWG82sfhnotRMw/CPa8N7nltKJi+w5ikV1u0aFGXDz2uqKjAvHnzjJuph0Q7F9KMGTNQWVmJfv36GXd9LcyU+Va63drHjN5YZjPiVa9o19jt+jcqXnX/JjIVEH1TJJUBqWtEMGXfDqQuByy5of1yu3ylrQeSZ2pz0H/e+EpZEEqXsgBI+73mWC8DNs3z+lLXiJeRzEcGfV29tJ9NfkZzrK3h9YpU5tSXRXt0R6R85EvWXaZJfib0OVkXWX/jZ6OVx1YZnlabj7ENZXqZxpIr2sO+Vfn8ViDlRX37yDTG86VN05MGDJ8Kf3sLzn30onHXbcPhnov8SeuRPmSicVeY3NKfIatwFhzuucZdPaY3tKEUj/bJHPlD5N1XheS0gbjyWTW+PLIZV8/vMiaLatGiRdi0aRNcLhcWL16MV199FRUVFcZkt6X58+dj2rRpvaa8iWDixIloaWkJe6g1Cb2xfXpjmc24FfWK9jeqoqICixYtwqhRo4y7etytqHtvlTABkbUY6PMTwJIN+GsAf62yTf+wdARbQ/uRBiQ/Lm6Wjfw14a+A8gDz5JmArQJAu7K9HrAOB1KeiX6TLW/ig16Rl5pvvdgeOBradl3ZlvwMkPz34t/+GiBwALCOBVJXKJlqaPOzDhftYS02porNWG9t3SXbOP17I7Wd5bnoojyBM+HtYJYlF0h7U7RH4ICSxxnAVg4kPxVKl7pCpAme1bRhMdDnf2lz6xkO91ykZhXiysn/MO66rdhzxmDAiGlIzRxp3BXm0pGN8DbvxZXTHxh39Yje0oZSPNona+TjAICm2udxctsMnNr+VLeCwdmzZ6OyshI+nw8tLS1obGxEQUEB5s+fD4fDYUx+23n//ffh8Xjw8ccfG3fR16CiogIulwt1dXXGXdRL26c3ltmMW1WvaH+j3G43KisrkZ+fb9zVo25V3XurhAmIbFPET98LgP8D4Pr/Azr/CFgL9D0TwYtAx2qgYwXQ/oNQgKHt3QGUNIaXv1rsSyoRP30viu2+pUD7M+Jn8LwuGx2r8mXB9Z0iLzXfnWJ74HhoW+fbYltypQgufC+EjuWvASyDwnu35Gd9S4GON0XAJ9ulO4z11tYdEIGgZVDkHh9JbWelrTv/KMqT9B19usCB8HYwK3he5Hvt50qdVwO+uaK95DkCgGurlTQLlTQLRXBkDM56QsZdlQj6vfhi380PobpdNP3Xj3F00/24dumIcVeP6G1tGI/2sdkd6Gg7jUuHf2fcZYrb7QYALFiwAK2trdiyZQtmzpyJhQsX9ooHh77++ut47rnnekVZE0F5eTm8Xi/+8Ic/GHdRL22f3lhmM25VvW7Hv1G3qu69Vdiy25ZcoM9cEQQASk+JT/R4eCeF0iVPB2yPAJYscQMcOABcWxO64U9dA1js4vPJfy9udoNnAf/7QOcmkcZaLIYmAUoexwD/n/U317HKY6sEUl5Qej2UG9jOP4Z6TXxLRdnSfg9c3y8CoT4/EeXx14h8Ov5FHNO+XfTC+DQjWWQZA/Uir9Q1IojStoVR6nJR3ms/B653Mb9bDvWSx5K9GYEz+uND6TlKeUGUt2N17O1myxypvtF0lY+WbgjbJXH8lAWx27mrumjJNGbykWkiiVUPSy6Q+i9A8Jgov1ZFRQXmz5+P+vp6LFt2c+uRpA+ZiKEPv4crn1Xj5LYZ6nbXY3tgTe6Hy8e3YuC3/gEWmx0dbafR2vAbNNevBAC457UBgBgmtvN/445xS5GSPkR9f+nw79T8ASDo96L94iF8eWQzWjz6cYYO91wMGDEN9pwxap5fNdXh1PankD9pPQaMmKZLr+V5XczZcbjnIu++qoj7tKIdS8orW4FM1w9gSxM9FV+dqcOZugURA4iu2tBM3c20oeuxPQCAxt+GujwjbcuftB723LFISR+ibvO3t+DguqGAyfaJdN59rYfwxSevhAU+kcqglTN2CQYWPw1bmgNBvxdXP/+rrg2rqqowfvx4LFmyBLNmzcKWLVtQU1NjzCYmOX6+paUFq1evxrPPPgun06m+79+/PxYvXozdu3ejpER8C7F582ZMmyauqYULF6KhoQEOhwMLFy7E+PHj1Xzb29tRWVmpPhy1oqICixcvVo8N5T94rVjl2bWre8MKo1m7di3sdjt27NiBadOmwW63o6mpCX/605+wceNGY/IujRo1Cr/61a8AAF6vF0ePHkV1dbXufEQ6VmNjIzZs2KDWKV75mDkXWvK4tbW1YX8TFy1ahG9961twOp3qtpaWFkyfPh34Gsose0ZlL+ju3bvx8ssv625aY6WJVJ5o572r9jFTdzPX89q1awEAc+bMUT9n3BapzMY21IpU5tLSUqxcuTKsHsbtva1e2u2IUmYz11isv1GLFi1CZaXh23WN8vJyzJ49G08++STeeecd3bA2Y9nNlFnL+HkKF9ZD1GepMsRIGZ5lHQQkKcGIlDwdSH5a/NtfIwIZ69jw4WeWQeIG1b9HBDKWLCD5R/pv3tXhUAdE+pQX9L0xZsoDAMgEOn+j9DKUAP46pQfkAbHbkgUE9gHJ/0O87/w1gFRlX5Rey8AB0aOATP12Oc9HvnR1Unoy+vwkfF8kltzQELfObnzha1HmxBmHqwUOKP8wlDleotVduq4JUM2QdQl6jXviz5Itricja7HoVUtdIXqwrkWY45WXlwe73Y7MzPDGdbjnYtjUbbhr8kbd/BD3vDbkT1qvSwsAA0vEH/UL+8Ufea2U9CHIdP0AbWfqcOWzaiSnDUTO6OfVOTxfHtkMX+sh2NIcyBr5ODoun8SVz6phS3PgjnGhX8Qvj2wW80s+/ytSMvKRd1+VrmzyRj0tu1CdixLwt2PAiGnIK1sBb/Ne9VhQghOZ55dHNqv5+C4dVrfJtEaxjgXlRt7x7R8DStmvfFaNvnfci6EPbzHkJkRrw1h1N9uGsTi/+5oaNGrb5lLj79U0ZtoHynlPHzIRl0+8j6/O1CE1q1Ati5zHlT9pPWxpDtjSHOp77fyunLFLcMdYMXzuyyOb0X7xEPoNnoA7K99VjyNvSH7605/C6XQiIyND3dcd1dXVaGxshMPhwPe//32cPXsWtbW1cDgcePbZZ9V0mZmZ2LBhA+x2O9xuN+rq6mC32/Hwww8DAJYvX47x48ejsbER1dXVyM3NxZgxImiWTp06herqavWYkZgtT7w4nU5UVlaivr4etbW1yM7OxqxZs7o9N0DWa//+/cjLy8PixYvD5h44nU6MGzcOdXV12L17N1wuV1id4pGPmXOh9eijjwJA2LfO8+bNU2/+ZLnkS+tWlXnGjBl48sknAeWYtbW1KCkpwerVoW/gzKRBN897V+0DE3WvjuP1HKsNtSKVedeuXWhqakJRUZEmJfC9730PAPCf//mf6rbeVC8pVpnNXGOx/kZ5PB7dvt27d6vpq5Xfi7feegterxfjxum/7Jo4Ufx97047a0WrOwk27RtLrvjm3Pite1ro/3UAQJIS8F77p9DNt/zW3VqsuSGHGNolv6kPzhRzcpK+I9IEDgAdmrSWXCDtbcB6N4Bq8+WBMpysc5MI1AJnlSBBuS60N+aWLBGgdW4S+dvKRU9WNMGLxi3KHCGNQEOo3v5qINgGJP9QpLNViICwc71+yJwlW+lNKg71WHXVoxSJJfSlW7cliy/oEDgb6lXpirHXJlrdpc63RS+dcdieZMnWLEKRqsw5agf8Ww0J4yx5unINGHqPtL2Vwdbw+khvvfUWGhoaIi5RnFv6M1hsdvjbW5BxZyUGjJgG38X/NiYDAPTJHIH0wRPw1Zk6tJ3+0LgbAPDF3pfVHo28shVwfPvHGDB8KtpOf6j23qRmFcLvbVF7WFyP7UFqViEAoO30h7q8+2SOwMjHP0Y/5wQ1X3kj31T7vK4XwuGeq+tNkce6crI6rIcJhmPJtEZmjpU16ke6nhVo6p458oe6z0VrQzN1N9OGZqRmfwsA8Pme5WE9OZKZ9pHOffSimnbY1G3oN3gCoJnHpaV9723ei7bTH2LA8KkAgNMfPK3mI+uUPmQi2k5/iJqaGly+fBmzZs1SbyAKCwuxZs2abg3xWLVqFRYtWgSXy4VLly5h1apVgPLNrcvlUtOdOHECGzduxLPPPotz587B4/GoN8sOhwMulwuNjY26b4M3bVKGEigaGhrQ0CC+/ZHHNDJbnmgifcurVV1dreYLAOvWrVO/lZXf7k6cOFEtayzaekFpj02bNmH8+PFh3/a+8soralrZyyfFIx+z50JyOBwYO3Ysdu/eHVbfgoICAMAbb7wR8dt63OIyT5kyRdc7Bc35Ki0txa5du0ylkcyc92jtY6bu8bietbpqQ61oZd6zZ4+6UIAsY1FREZqamtS26Y31ilVms9eYNp9If6NqampQU1Oj7qutrQ27zgGgvr4e5eXlGDVqlJpfQUEBvF5vt9pZu6+rulOIroco6dviZ+C4dqsYaqYlgxTtTaP8jHVwaBuU4ECS815kAGLJFYsCpCorrskeJusg8dNseWLRlskySAy5gzLHxIxIAZN3kv5lvMG+/pEI4jr+RbSVrTx8oQNLFmAZrrRjO2Adpt8fS6RALRrZo5O6XOnhawf8f9IvXBDpZeyBilV3KXBAP1dHy5IVChZt5UCwHbj2z+bPyY1IKhM9lMGzoWtRChwQdWmfKepjmxDe4ynt2rUr7KbR4Z4Li82Olk9fw8F1Q9Hy6WtIychHVuEsBP1etB7+jS7939z9Y1hsdrQe/jfddi1t4CEnzFtt4Utlepv3qv9u/O04dShWn8wRcH73Nbge2wPXY3vUHoKUjFCXaFp2IXyth8Ju5CMFPTfLzLFS0ofAluZQl5J2z2tTe4xsfbI0n4rehmbqrtVVG5px5dR2BP1eDPm7f8WomQdx1+SNyBm7xJjMNG0g5/eGrrNT25+C5/V0eF5Ph6/1EHyth9T3ntfT1XZMzRLtrM3Hd0H0SmkXxdi1axfmzJmDxsZGtLS0oLy8POyb8O7weDzqv+fMmRNxeFUk99xzD6AETVo3+4yMGy2P9lveSC9tvlBuciQ5xKVv376aFNE5HA7MmzcPa9euxdq1a7F8uVjFJzc3fAUe7c3MpUuXdPvikU93z8Wjjz4Ku92OrVvDv8nauXMnvF4vVq5ciXfffRfLli3DjBmhYa24xWV2Op1wOByora1VX7I3qH///qbTSGbOe7T26U7dcRPXs1ZXbagVrcyyd0Eeu7S0FA6HA3v2iCG86KX1ilVms9dYvMh2lr06UOZ97t8fuvmNVWataHWnkLAhc7dS6gqxKEDgrAh6jIFPvATFVAHx77OAVbmvirbim2TJ1QdR3eWvFoGRvzZ8oYHAUbFwg2+pGOJnLQhfvCGa4Bfip1yMQVLrZfi7IAMQ2Yt37Z81PXURFkpQFzPoIuCJpbNGHEu2t1bgaCigCtSLACl4WeyTS2fLXixJDquLpqs0SWViCGOwVSx20ZXgeaVXc0+ox9MMOSRK3oSe++hFHFw3FCf+fSr2v5kT1oORcddDEYODeBr68BZkjpiBjiun4LtwSL0pvhEB/1fGTT3G27wX5/6yOOxlXJUtWhvGs+5G1mT9RdZcvxKNf7gPLZ++ho7LJ2HPGYM7xr6IUTN75j/LnrBu3TrU1tbC6XSitLTUuDuhNDQ0YNWqVV2+jN++3qzVq1fjwQcfxPnz53HixImwmy6z4pVPd0yYMAGNjY0Re4A2btyImTNn4p133sHZs2dRVFSEZ599Fu++Gxq6eavL7PF4UFVVFfbSrgRmJo1Z0dqnJ+tut0f4FtekaGVuaWmBx+NR5wPK4XIffhj6/6031qsnyxzJ1atXjZt0Ghoa4PF4MHasmB8iv0j45JNP1DTdKXO0ulOILiAKnFE2Kj00kvFb/sDR8JtF2bsh85C0N/jaG1xbpQgQOn8jVhnrWB0+f8ZseWLRDkOTq4clzxSLNcQi03SnVypaoGXp4ovnzt+JHhvbZOOervmrxWeSxuqPmfxD8fO6YZ6M2qvzfbGSWneG592I6x+JACRWUCHnXKUoX4bI855k6PWW7+X+wFEx9E5bd4sYpaEGwZZc0SvW52fKghUvmuuFsmYbt4TIb8W02pRhbMbAx/geyhAwW5oDXx4Tk/67op3v0t0eB4d7LlLSh6D5k1fUZZk//6tYkEGr/eIhpGYVInOkctF0wXfxMAAgOd3wy9gNZo7V0XZazDE6/QFaPGt0L+2iCtHa0GzdzdIGQH0yR+gWTpCuXTqCcx+9iOPvTcbBdUNx5bNqMQ8sSl17iq9VtLP2mVGpA8UQPd8lcR6N16+W8Zvwnnbq1ClAmZ+nZZyrcLvSjtk39oDEUlFRAafTiQ0bNmDZsmVYtWrVDT0fJF75dOdczJ49Gw6HQ3czbNSiPO9k8eLFmD59ui7ovtVlbmpqQkFBAT7++GN16JJ8yR5/M2mkWOc9WvvEq+6SNlBwOBxwahax6I5oZZY8Hg/sdjtmzJiBoqIieDwetYemN9bLTJnNXmNmySH3xvy0du7cCbvdjtmzZ2P06NHwer3qoh1myixFqzvpJaWkpKjLTQS/EDed1lFiuJr1W2KIkcUOWNKATuWLHUtfIOkeIOlewDoESJ4mPhM4KubJAIDtIXGzah0CWIuApPuA5AcBJAMdvwKCVwDb9wBLBoAgkHS3eE4P2sQ2y0Dg+vuxy2MtAJJKxcIO13cByU+IfwcvGLZPA4JXgc5/B2zfBZJGA9cPiOffaD8LiyhzUimQ8pyy/wDQ8X/09bI4RBrtyzJA5JX2f4Hkh5R63yv+nfQdEbxceymUDyBW3QMAfAVY8oCkcaI3KqD5QttYRy1LHpBULIZ4WYcox5ogAr9r/yjSyDLL83ejzNTdWC/LwFAAe323SJP8hPIcIiVN4JhynkuA658qQ+2+LQKppPGAdaSyGMcosU+9DoeI82gbKwJy2c7Bs0CHsgJz6j+G2v76PtFWxjKnLhfXhPXbynn/n8p511zP0uzZs7Fw4UK4XK4b/qZ48P2/RDDQgZPbDF1gCrk6WJ+sEUh3liNzxHRkuX4AizUZ53a+iP53PgiH+1mkDiyELc0BS1IyMoY8gEDnV+i4fBIAkNQnQ1mpLRtWax+k5/8d8spW4HrHZST16Y/UzOG4crIawUAHMoZMxIDhf49+ed9BxpAHMGDYVAwsfhqXDv9WLdP1jsvILnwC9r8ZDfsdY9H/zgcxYNhUWJPt8F34b+SVrUDWyB9hwLCparlSB4zAgGFTkdJvMLzNfzV1LAssyLirEtmFT6Df4HI1Tdaox/HlkdB47WhtaKbufTKGxmxDABgwbCrSHG5k5E9C+uByDHTPgb+9RdRPacP8SeuRNepxtU0GFj+Nfnl/CwQ6capGTKIz0z7yvMuVBOXxU7MLddugXCMAcPHA/9VtBwBbmgP9Bt2H9CETYXd8G38z+nmkOdzwtR5Sh16+/fbbePjhh+F2u5Gfn48777wTY8aMgdfrxT/+o/KHI4aKigo88sgjGDp0KAYOHAibzYZ77rkHra2tuHDhAgBg+PDhKCsrw7Fjx7Bz507MmjULx44dQ3Nzs7r9vffeQ2lpKYqKinD33XfD7XbjySefRFpaGvr27YsNGzYAyu/epEmTUFZWph4zJycHZWVlSE9Px/Dhw2OWJ56mTJmCgQMHIj8/H263G+Xl5XjooYeQnJyM1atXmzpmcnIyJk+ejIyMDPj9fowePRrz58/HlStXkJ6ejpycHNTX16vHkm0BAGVlZSgoKMCGDRvils+FCxdMnQsoS7Z3dHR0uWLVokWL8MADD2DcuHEoKyvDlClTMHr0aHR2dmLVqlW3vMzt7e24//77MXnyZBQXF+Oee+5BWVkZHnjgAdQqi4yYSWP2vEdrHzN1z8rKMnU9l5WV6er+yCOP4OLFi8jKyjLdhlK0Mkv79u3DjBkz4HQ6kZubi+3bt2Pfvn1AL62XmTK///77pq6xWH+jZCB0+fJlTJ48GYWFhSgoKFB/RwKBAM6cEd/4Hjx4EA899BCys7MxaNAgHD58GH/+859Nl7m+Xjy4MVrdSS9syNy15eKm01oshlcFzoYeAip1blJWaVOGYVmHi2FP1yI9wLRW3BDLeSKdvw4N0+r8N2Vy/QtiCW9/rbhRtmSFls02Ux4zAgdET0rwgngm0LWfi14p7yT9ggHauS1oF0t4+xZqcxLU+S+al/ocIaU3yVYePkQtGrWX6BHjnq51rFae4SPPRbGy3HaUYWE3y1hvbd2NzC6S4N8mfspeomu/UB7YOljJf7B4f+0Xoc90vinmOCEtSt2VlQRlmkhlDnhD15etIrTARaTr+dy5c/B6vV2OU45F9l5oVyDryuXjW2HPGYOMOytxvfMqPq9fgbbTH4YekqpMzO83eELYQ1PbTn+Ilk9fgy3Ngbz7qjCw+GlcPr4Vfu8XYlW1wlkAgEuHf4em2ufhbd6LvnfciwEjpom8svWT/q9dOoLzu36OzvYL6oIR2gn96UMmhj6rlEu+l0tsmzlWi2cNzv1lsboymkxjtWm+KYzRhmbqbqYNAeBM3QJ4m/fCnjMG/Yc+iNaD7wBK0CHb0GZ36Nqk7x33ov3iITTVPq/mY6Z94qW5fiU+rxcTFgeMmIa07EJ8daYOn1U/oaaRY9/Ly8vVb149Hg9eekn5xsYE+XBBOXF4/PjxN/ywwaVLl8Lj8ah5nj9/Hnv3huZ1AcC4ceNQWVmpO6Z873a741qe7tixYweKiopQXl6Oq1ev4o033jA9cbmhoQHvvPMOsrKy1F6UHTt2oLW1FQ6HQ12ePJZ45QOT50J+Qy1XxookMzMT5eXl6jkqKSnB0aNH1WvsVpe5pqYGVVVVOHr0qHptVFZWIjVV/idhLo0U7bzHah8zdTd7Pb/88stq3SdMmIAtW8SKnN1tw1hl1tq/fz+cTie8Xq+uZ6I31stMmWHyGov1N0pqaWnBL3/5S1y8eFH3O2K0d+9euFwuOBwOHDkSGiFhtsyx6k56Yc8hipdYz3q51eQqYsGzSuD1hZhvIp+JRHQrFEzfgbTsQjT+4b6Iz9WBZkWw7kzsTyRm2pDMW7t27Q0/hyiRyRWxbmQSeG/36quvoqCgADNnzgwbSvZNZ+a898b26Y1lNqO316uqqgolJSU3VP7eXvdbLayH6JsqcEDp1UoTS3+nvBB6lhLRrdJx+TM0f/IKb+RvAtuQ6Ot17tw5bNiwgTdZXeiN7dMby2xGb67X7NmzMX78eNTV1d1Q+Xtz3b8OCdNDpJVUJhY3CLb1/MICRN3FHiKi25+ZngL65uF5p55UUVGB8vJyDBo0CE6nE01NTXjiidBwZ+o5CdNDpHX9I7FCG4MhIiIiIroduN1ulJSUwOv1YvPmzQyGbqEe6yEiIqJvrvPnz0d8CCAREVFvk5A9RERERERERGBARHR7yJ+0vtsPXyU9tuGNWbt2re4hk0RERInGVECUsgCwbzdu/frcbuUhuhk5Y5dgwIhpSEr5Ziyi4HDPhfO7ypNxb5He1Ibxah+Hey5GzTwI97w2uOe1oWD6DmMSIiIiMsHUHKKUBeKBlbfLinE3Wp6kMiD5h2L1O0B5mOwaIHhevDcGWfKZRZ1vh7bJ1fMi8deEHvKaskA8CNaSJd4HDgD+P4vFHKDkAwC+ucqHFfbtysNGlQegdiVwNPTZ5GfEQ2AtWeLBroED+npFKnPgANC5pXsLS0TKR5J1l2k6/ygenArN+er4F1F/YzsjSnlslWKJdC1tPtp2gCa9TGPJBfrMFc+hQppoH/8eoHN9qH1kGstw/fm69otQmp7kemwPbGkOHFw31LjrtuFwz4U9ZwxaD/8Gbac/NO7WKXmmGRabHef+shgtHuVC72G9oQ2leLRP5sgfYsjf/SuCfi/aztQh0HEVnd7zOPeR+ScyL1q0CGPGjIHD4QAAeDweVFdXm34eEecQERHRN4WpHqJvAmsx0OcngCVb3Lz7a5VtS/Xpgq2h/fKZRanL9WmgBADGV0B5OHnyTCWYaVe21wPW4UDKM+Lmuys25UHFQa/IS823XmwPHA1tu65sS34GSP578W9/jbiRt44FUsWD6nW0+VmHi/awFhtTxWast7bukm2c/r2R2s7yXHRRnsCZ8HYwy5ILpL0p2iNwQMnjjAgek58KpUtdIdIEz2rasBjo87+0ufUMh3suUrMKceXkfxh33VbsOWMwYMQ0pGaONO4Kc+nIRnib9+LK6Q+Mu3pEb2lDKR7tkzXycQBAU+3zOLltBk5tf6pbwdDs2bNRWVkJn8+HlpYWNDY2oqCgAPPnz1cDJCIiokSRMAGRbYr46XsB8H8AXP9/ohfDWiB6jqTgRdHT0bECaP9BKMCQwYrUsTr8JXt/kkrET9+LYrtvKdD+jPgZrcfBOkr8vL5T5KXmu1NsDxwPbZO9VsmVIrjwvRA6lr8GsAwSgZmW/KxvKdDxpgj4ZLt0h7He2roDIhC0DNK3q5Hazkpbd/5RlCfpO/p0gQPh7WBW8LzI99rPlTqvFr1JwdbQOQKAa6uVNAuVNAtFcGQMznpCxl2VCPq9+GLfzQ+hul00/dePcXTT/bfswam9rQ3j0T42uwMdbadx6fDvjLtMcbvdAIAFCxagtbUVW7ZswcyZM7Fw4UI+xI+IiBJOWEBkyRU9Ivbt4pXSxZeOydOBtN8r6baKz2h7P1LXAGnrxU25fatIl7ZefE6yFoeOY98KpL4cHnjEKo+tUmxPXa4cZ6vmmFtDN7VJJWKolHWYSNvnZ6K3CBAPae1Kxwbx02a4UY+qXfywDgttCp4XN/ddseQCtgmiFyhaOi1bpQgirtfrAy2/8sVzUhfD24BQAGMdZNxz8wJnRD2Sowz5Mwp+IX5a7MY9N6fz7fBheMGLoaFxUIIubRpLrmjXSD1SFRUVeP/997Fs2TLjrm5LHzIR/QZPQNuZOt3NseuxPRg18yDyylag5JlmuOe1YdTMg7oFA+S8kaJ/OIHMkT9U55LI9zJ/ma7kmWYUTN8Bh9swRlPpYSmYvkOXZ/6k9YCyUIF7XhsGjJgGAMi7r0pN557XpstDu127TyvasaS8shUo+ocTapphU7ehT+YIXRqpqzY0U3dtGbpqQ9dje+B6bI/uc5G25U9ar5vPI/ORzLRPpPPuemyPWhajQOdXxk2qnLFL1DYseaY5rA3b28UfqeHDh6vbWlpa0NBg6OolIiJKAGEBUZ+lyhAjZXiWdZCYC6OVPB1Iflr8218DBI6JzxiHn1kGiZt2/x4xLMqSBST/SP/Nuzoc6oBIn/KCPigyUx4AQCbQ+Rull6EE8NcpPSAPiN2WLCCwD0j+H+J9568BpCr78kPZGAUOiB4FZOq3pyzQv3R1Unoy+vwkfF8kltzQELfObnzha+knfhqHq6kBlaHM8RKt7tL1+sjbuyLrEvQa98SfJVtcT0bWYhFMp64QQdO1CNM78vLyYLfbkZkZ3rgO91wMm7oNd03eqLv5ds9rC7vpB4CBJXMAABf2rzXuQkr6EGS6foC2M3W48lk1ktMGImf080gfMhEA8OWRzfC1HoItzYGskY+j4/JJXPmsGrY0B+4YF/pF/PLIZnx5ZDOufv5XpGTkI+++Kl3ZHO65yLuvCmnZhbjyWTW+PLIZAX87BoyYhryyFfA271WPBQBfnalT8/zyyGY1H9+lw+o2mdYo1rGg3Mg7vv1jQCn7lc+q0feOezH04S2G3IRobRir7mbbMBbnd19TA0Zt21xq/L2axkz7QDnv6UMm4vKJ9/HVmTqkZhWqZXG45yJ/0nrkT1oPW5oDtjSH+j5/0nr12sgZuwR3jBXfHH15ZDPaLx5Cv8ETcGflu+pxamtrAQA//elP4XQ6kZGRoe4jIiJKNLqAyJIrhpDJiepyiJFRUrn4ee2fQkOMAkfFZ403wZ1viyFRkYZFaYdD+ZaKYV8AYL1b/DRbHijDyTo3Kf8+qw8StGWyZCmT6jeJifUw0SsRvGjcIuYIaV/WwaF9/moxBCtwRuxLfVn0bBnnD1myRW9V2psiGPTXhfdmRGNxGreYJ3vqAmdDvWxdvVIW6D8bre6SOqTPMGxPsmRrgqoXRaCMdsC/1ZgyvpKni2tAzsGSrMXiPCU/rvQOHdfvl9566y0sWbIEy5eHTyzLLf0Z+g2eAHvOGOTdV4WC6Tu6XE2sT+YIpA+egK/O1HW5SMEXe1/GyW0zcHLbDFz473Ww2OwYMHwqAODU9qfguyBurP3eFhx/bzJObpsBX+shpKQPAQC0nf4Qp7Y/hVPbn8Lx9ybj2B9Fl10/5wT1GPJGXjsXpeHtIpz7y2Kc++hFtHjW6I515WS1muep7aGJWNpjybRGsY4FAFmjfgR/ewsOrhuKU9ufUuuekj4krKckWhuaqbuZNjQjNftbAIDP9yzXtY12To+Z9pHOffSiWu6vztSpZZHzuAaMmKYGRPK9dn6XvEZOf/A0Tm1/Ckc33Q9f6yGkZhWqQVNNTQ2WLFmCpqYm2O12PPvss1i2bBnnDxERUULSBURJ3xY/jTeD1/fr38sgRTu0S37GeHOsnVsib5JlAGLJFYsCpK4RL9nDJIdxmS1PLNoyWQYB8Il/R5vPoxUpYPJO0r90c2ggAhvfXLHaWeComMhvXOjAkiVWNgscEMGAdoidGZECtWhkAJK6XOnhawf8f9IvXBDpZeyBilV3KXBAP1dHy5KlCarKgWA7cO2fzZ+TG5FUJgKv4Fn9yoFQyuqdBLTPFPWxTQjv8ZR27doVNs/C4Z4Li82Olk9fw8F1Q9Hy6WtIychHVuEsBP1etB7+jS7939z9Y1hsdrQe/jfddi3tCmTy5tpqU7rSNLzNe9V/N/52HDyvizGgfTJHwPnd19QhXrKHICUj1CWall0IX+uhsLkoN7r6WTRmjpWSPgS2NIduaJnsMbL10YxzjNGGZuqu1VUbmnHl1HYE/V4M+bt/xaiZB3HX5I039TwkbXDn94aus1Pbn4Ln9XR4Xk+Hr/UQfK2H1Pee19PVdkzNEu2szUcGYdpFMXbt2oU5c+agsbERLS0tKC8vx+rVyjKZRERECSRsyNytlLpCLAoQOCuCHmPgEy9BzXD94FnAqtxXGXtsIrHk6oOo7vJXi8DIXxu+0EDgqFi4wbdU9A5ZC8LnUEUj593IxRgktV6X9NvVHp1iEQBc+2fxU9tTF+nVVcATS2eNOJZsb63A0VBAFagXAVLwstgne6y0882A0LC6aLpKk1QmhjAGW8ViF10JnhfBkn9P5B7PrsghUfIm9NxHL+LguqE48e9Tsf/NnLAejIy7HooYHMTT0Ie3IHPEDHRcOQXfhUMxeyaiCfi7nq8Sb97mvaLXyPAyrsoWrQ3jWXcja7L+ImuuX4nGP9yHlk9fQ8flk7DnjMEdY1/EqJkHdeluZ+vWrUNtbS2cTidKS0uNu4mIiL7RdAFR4Iyy0TDR3vgtf6ThcbJ3Q+YhaW/wtTe4tkoRIHT+RhlStzp8/ozZ8sSiHYYmVw9LnimePROLTNOdXqlogVZXCzh0/k702NgmG/d0zV8tPpM0Vn/MZGVk0XXDPBm1V+f7Yphjd4bn3YjrH4kAJFZQIedcpTwqfsrznjQ+lEb7Xu4PHBVD77R1tygLScgg2JIresX6/Ex8zveiuV4oq7LgRiSlpaVhQ4vkkChj4GN8D2XRAFuaA18ee8+4S0c736W7PQ4O91ykpA9B8yevqMPTPv/rSmMytF8UQ6mMw9GMfBcPAwCS0298FQ4zx+poOy3mGJ3+AC2eNbqXdtGEaG1otu5maQOgPpkjIg6nu3bpCM599CKOvzcZB9cNxZXPqiMO87sVjMPjACB1YKHYd0mcR+P1q9W/f3/jJiIiom+0sAezygdrBg6InhvrMOWmMyv0IFS5qEKwVZk8P0jpddA8JFPmEzwbujG3jRPzM3wLlTQvK4slbBPf7NseVAqRpjwQ9c3Y5ZEP4vQrDwa1Kw82DTQYtm8VvTD+D5TnCqWJfbYK/WdlnYDQg1UDBzRlVsrjj/DswkCDCFLSfi8CletHRc+SNUssDIF2EYygiwezygeYdv46NB8KmoeNynJqyc+o50I5VvAs0K5M8ZBl7u6DbI3M1N1YL+1zkqI9UFXm7Vso2jv15dA1FTguzru8DuS5kHkHzwLXD3RRdyUftCsLbWioZVamAwVaxc+kYhGsG8sI5fktTz75JDweD5577jn9TpNGzTwIqy2ty4eIuh7bg9SsQnS0nYbvouhlSB88ARabHSf+fSpSM0fCnjMGqQMLkZpViK/O1MHvbdE9NDV9yEQMffg9+FoPofXgO7D2yUDWqB8BAKy2NFw5+R9o+q8fI3PkD+EsfwUWm13NB8qyzsffC0XnfTJHwPXoXwBAfRAoAFw5vR2XDv8OeWUrkGwXkaksl1x0wdu8Fy2eNaaOJRdeCPq9uPr5X9U01pS+OLltBqRobWim7r6Lh2O2IQAMm7oN/QZPgLd5Lzouf6YGFrY0h9qG+ZPWw5rSV20Tm92BvnfcCwDY/2YOoARwsdpHnnftcL38SesxYMS0sCF8cpW7xt+GP/BLLqrgb2/BV011SOl/J+w5Y+BrPaSm37RpE3w+H44fP46ioiK0trbC5XLB6/XiwQflH+Lo+GBWIiL6pggbMndtubjptBaLG+3A2fAJ6J2blFXalGFY1uFi2NO18Hnm8NeKHh05T6Tz16FhWp3/pkyufwGwPSLSBluV1eiUm2gz5TEjcEAEOMEL4plA134uggvvJH2QoZ3bgnaxEIS8AdcyLixgq9A8R0jpTbKVhw9Ri0btJXrEuKdrHauVxSrkuSgW5yLasLCbZay3tu5GZhdJ8G8TP2Uv0bVfKA9sHazkP1i8v/aL0Gc631SCs7QodVdWEpRpIpU54A1dX7aKULAc6Xo+d+4cvF4vLl0yjEc0SfZeaFcg68rl41thzxmDjDsrcb3zKj6vX4G20x+GHpKaJW7O+w2eEPbQ1LbTH6Ll09dgS3Mg774qDCx+GpePb4Xf+4VYVa1wFgDg0uHfoan2eXib96LvHfeGJuhni7yla5eO4Pyun6Oz/QIy7qxU00npQyaGPquUS76354wBTB6rxbMG5/6yWF0ZTaax2kIT+WK1oZm6m2lDADhTtwDe5r2w54xB/6EPovXgO4ASEMk2tNkdujbpe8e9aL94CE21z6v5mGmfeGmuX4nP68WExQEjpiEtWwR8n1U/oaY5eFAE2uXl5XA4HHA6nfB4PHjppZfUNERERIkirIcoXuLVKxEvchWx4Fkl8PpC9Eppe2KIelrB9B1Iyy5E4x/u6/LBnJF6CijETBuSeWvXrsWWLVtQUxOh6zcK9hAREdE3RVgP0TdV4IDSq5UmllZOeSH0LCWiW6Xj8mdo/uQV3sjfBLYhERERxVPC9BBpJZWJxQ2CbT2/sABRd7GHiHoD9hAREdE3RcL0EGld/0hMpmcwRERERESU2Hqsh4iIiIiIiOh2l5A9RERERERERGBAREREREREiYwBERERERERJSwGRERERERElLAYEBERERERUcJiQERERERERAmLARERERERESUsBkRERERERJSwGBAREREREVHCYkBEREREREQJiwERERERERElLAZERERERESUsBgQERERERFRwmJARERERERECYsBERERERERJSwGRERERERElLAYEBERERERUcJiQERERERERAmLARERERERESUsBkRERERERJSwGBAREREREVHCYkBEREREREQJiwERERERERElLAZERERERESUsBgQERERERFRwmJARERERERECYsBERERERERJSwGRERERERElLAYEBERERERUcJiQERERERERAmLARERERERESUsBkRERERERJSwGBAREREREVHCYkBEREREREQJiwERERERERElLAZERERERESUsBgQERERERFRwmJARERERERECYsBERERERERJSwGRERERERElLAYEBERERERUcJiQERERERERAmLARERERERESUsBkRERERERJSwGBAREREREVHCYkBEREREREQJiwERERERERElLAZERERERESUsBgQERERERFRwmJARERERERECYsBERERERERJSwGRERERERElLAYEBERERERUcJiQERERERERAmLARERERERESUsBkRERERERJSwGBAREREREVHCYkBEREREREQJiwERERERERElLAZERERERESUsBgQERERERFRwmJARERERERECYsBERERERERJSwGRERERERElLAYEBERERERUcJiQERERERERAmLARERERERESUsBkRERERERJSwGBAREREREVHCYkBEREREREQJiwERERERERElLAZERERERESUsBgQERERERFRwmJARERERERECYsBERERERERJSwGRERERERElLAYEBERERERUcJiQERERERERAmLARERERERESUsBkRERERERJSwGBAREREREVHCYkBEREREREQJiwERERERERElLAZERERERESUsBgQERERERFRwmJARERERERECYsBERERERERJSwGRERERERElLAYEBERERERUcJiQERERERERAmLARERERERESUsBkRERERERJSwGBAREREREVHC+v/ofYbR2PQuGgAAAABJRU5ErkJggg==)

![[Screenshot 2024-12-27 164159.png]]

![[Pasted image 20250108213542.png]]

![[Pasted image 20250108213602.png]]

![[Pasted image 20250108213630.png]]
![[Pasted image 20250108213645.png]]
![[Pasted image 20250108214301.png]]

![[Pasted image 20250108213700.png]]
![[Pasted image 20250108213728.png]]
![[Pasted image 20250108213750.png]]
![[Pasted image 20250108213756.png]]


It looks like you've posted the help message for the `gzip` command, which is used to compress and decompress files. Below are some examples of how you can use `gzip`:

### 1. **Compressing a File**:

- **Command**: `gzip file.txt`
- **Explanation**: This will compress `file.txt` and replace it with `file.txt.gz`. The original `file.txt` will be deleted by default.

### 2. **Compressing a File but Keeping the Original**:

- **Command**: `gzip -k file.txt`
- **Explanation**: This compresses `file.txt` to `file.txt.gz` but keeps the original `file.txt` unchanged.

### 3. **Decompressing a File**:

- **Command**: `gzip -d file.txt.gz`
- **Explanation**: This decompresses the `file.txt.gz` file and restores the original `file.txt`.

### 4. **Decompressing and Keeping the Compressed File**:

- **Command**: `gzip -dk file.txt.gz`
- **Explanation**: This decompresses the file `file.txt.gz` but keeps both the compressed and decompressed files.

### 5. **Compressing a File and Writing to Standard Output**:

- **Command**: `gzip -c file.txt > file.txt.gz`
- **Explanation**: This compresses `file.txt` and writes the compressed output to `file.txt.gz` without deleting the original file.

### 6. **Listing the Contents of a Compressed File**:

- **Command**: `gzip -l file.txt.gz`
- **Explanation**: This shows information about the contents of `file.txt.gz`, like its original size, compressed size, and compression ratio.

### 7. **Testing a Compressed File for Integrity**:

- **Command**: `gzip -t file.txt.gz`
- **Explanation**: This tests whether `file.txt.gz` is a valid gzip file without decompressing it.

### 8. **Compressing Files in a Directory Recursively**:

- **Command**: `gzip -r directory/`
- **Explanation**: This will recursively compress all files in the specified directory and its subdirectories.

### 9. **Using a Custom Suffix for Compressed Files**:

- **Command**: `gzip -S .gz2 file.txt`
- **Explanation**: This compresses `file.txt` and gives it the `.gz2` suffix instead of the default `.gz`.

### 10. **Compressing Files with the Best Compression Level**:

- **Command**: `gzip -9 file.txt`
- **Explanation**: This compresses `file.txt` with the highest compression level (slower, but more efficient).

### 11. **Compressing a File for Rsync**:

- **Command**: `gzip --rsyncable file.txt`
- **Explanation**: This compresses the file `file.txt` in a way that makes it more efficient for use with `rsync` (which can save bandwidth during file synchronization).

Tar file


You can replace `file.txt` and `directory/` with your own file and directory names

It looks like you've pasted the full help message for the `tar` command. Here are a few examples of how to use `tar` in various scenarios using the command:

1. **Creating an Archive**:
    - **Command**: `tar -cf archive.tar file1 file2 file3`
    - **Explanation**: This will create a tar archive named `archive.tar` containing `file1`, `file2`, and `file3`.
2. **Extracting an Archive**:
    - **Command**: `tar -xf archive.tar`
    - **Explanation**: This extracts the contents of the `archive.tar` into the current directory.
3. **Listing the Contents of an Archive**:
    - **Command**: `tar -tvf archive.tar`
    - **Explanation**: This lists all the files inside `archive.tar` in a verbose format.
4. **Appending Files to an Existing Archive**:
    - **Command**: `tar -rf archive.tar newfile1 newfile2`
    - **Explanation**: This adds `newfile1` and `newfile2` to the existing `archive.tar`.
5. **Extracting Files to a Specific Directory**:
    - **Command**: `tar -xf archive.tar -C /path/to/directory`
    - **Explanation**: This extracts the contents of `archive.tar` into `/path/to/directory`.
6. **Extracting Specific Files from an Archive**:
    - **Command**: `tar -xf archive.tar file1 file2`
    - **Explanation**: This extracts only `file1` and `file2` from `archive.tar`.
7. **Compressing an Archive with gzip**:
    - **Command**: `tar -czf archive.tar.gz file1 file2`
    - **Explanation**: This creates a gzipped tar archive named `archive.tar.gz` containing `file1` and `file2`.
8. **Using Wildcards**:
    - **Command**: `tar -cf archive.tar *.txt`
    - **Explanation**: This creates a tar archive named `archive.tar` containing all `.txt` files in the current directory.
9. **Excluding Files or Directories**:
    - **Command**: `tar -cf archive.tar --exclude='*.bak' .`
    - **Explanation**: This creates a tar archive but excludes all `.bak` files from being added.
10. **Extracting Files from a Compressed Archive**:
    - **Command**: `tar -xzf archive.tar.gz`
    - **Explanation**: This extracts the contents of a gzipped tar archive.

![[Pasted image 20250108214016.png]]
![[Pasted image 20250108214023.png]]

![[Pasted image 20250108214035.png]]
![[Pasted image 20250108214048.png]]

![[Pasted image 20250108214106.png]]
![[Pasted image 20250108214121.png]]

![[Pasted image 20250108214137.png]]

![[Screenshot 2024-11-20 091138.png]]
![[Screenshot 2024-12-31 123314 1.png]]
![[Pasted image 20250108214330.png]]

![[Pasted image 20250108214339.png]]

![[Pasted image 20250108215038.png]]
![[Screenshot 2025-01-07 124556.png]]
![[Screenshot 2025-01-06 171450.png]]


![[Screenshot 2025-01-05 180542.png]]

![[Screenshot 2025-01-06 173703.png]]
- `>`: Redirects output (overwrites the existing content).
    
- `>>`: Redirects output (appends to the existing content).
    
- `<`: Redirects input from a file.
    
- `2>`: Redirects error output (overwrites the existing content).
    
- `2>>`: Redirects error output (appends to the existing content).
    
- `&>`: Redirects both stdout and stderr (overwrites the existing content).
    
- `&>>`: Redirects both stdout and stderr (appends to the existing content).
    
- `|`: Pipes output of one command to another.
    
- `<<`: Here document for multi-line input.
    
- `<<<`: Here string for single-line input.
    
- `/dev/null`: Discards output.

### File and Directory Management:

- `ls`: List directory contents.
- `cd`: Change directory.
- `mkdir`: Create a new directory.
- `rmdir`: Remove empty directories.
- `rm`: Remove files or directories.
- `cp`: Copy files or directories.
- `mv`: Move or rename files or directories.
- `touch`: Create an empty file or update file timestamps.
- `cat`: Concatenate and display file content.
- `head`: Display the beginning of a file.
- `tail`: Display the end of a file.

### File Permissions:

- `chmod`: Change file permissions.
- `chown`: Change file owner and group.

### System Information:

- `pwd`: Print the current working directory.
- `whoami`: Display the current user.
- `uname`: Display system information.
- `df`: Display disk space usage.
- `du`: Display disk usage.
- `top`: Display tasks and system information.
- `ps`: Display current processes.
- `kill`: Terminate a process.
- `uptime`: Display how long the system has been running.

### Network:

- `ping`: Send ICMP ECHO_REQUEST to network hosts.
- `ssh`: Open SSH connection to a remote host.
- `scp`: Securely copy files between hosts.
- `wget`: Download files from the web.
- `curl`: Transfer data from or to a server.
- `netstat`: Print network connections, routing tables, interface statistics.
- `ifconfig`: Configure a network interface.
- `ip`: Show/manipulate routing, devices, policy routing, and tunnels.
- `traceroute`: Print the route packets take to the network host.

### Disk and Filesystem:

- `mount`: Mount a filesystem.
- `umount`: Unmount a filesystem.
- `mkfs`: Create a filesystem.
- `fsck`: Check and repair a filesystem.

### Text Processing:

- `grep`: Search text using patterns.
- `awk`: Pattern scanning and processing language.
- `sed`: Stream editor for filtering and transforming text.
- `sort`: Sort lines of text files.
- `uniq`: Report or omit repeated lines.
- `wc`: Print newline, word, and byte counts for each file.
- `cut`: Remove sections from each line of files.
- `paste`: Merge lines of files.
- `diff`: Compare files line by line.
- `comm`: Compare two sorted files line by line.

### Compression:

- `tar`: Store and extract files from an archive file.
- `gzip`: Compress files.
- `gunzip`: Decompress files.
- `zip`: Package and compress files.
- `unzip`: Extract compressed files.

### Package Management:

- `apt-get`: Package handling utility in Debian/Ubuntu.
- `yum`: Package manager for RPM-based distributions.
- `dnf`: Package manager for RPM-based distributions (successor to `yum`).

### User Management:

- `useradd`: Create a new user.
- `usermod`: Modify a user account.
- `userdel`: Delete a user account.
- `passwd`: Update a user’s authentication tokens.
- `groupadd`: Create a new group.
- `groupdel`: Delete a group.
- `groups`: Show group memberships.

### Miscellaneous:

- `echo`: Display a line of text.
- `date`: Display or set the system date and time.
- `history`: Display the command history.
- `alias`: Create an alias for a command.
- `unalias`: Remove an alias.
- `crontab`: Schedule periodic background jobs.
- `at`: Schedule a command to run once at a particular time.
- `man`: Display the user manual for a command.
- `info`: Display command documentation.

### Common Unix/Linux Commands:

### File and Directory Management:

- `ls`: List directory contents.
    - `ls -l` (long format)
    - `ls -a` (include hidden files)
    - `ls -h` (human-readable file sizes)
    - `ls -r` (reverse order)
    - `ls -t` (sort by modification time)
- `cd`: Change directory.
    - `cd /path/to/directory` (change to specified directory)
    - `cd ..` (move up one directory)
    - `cd ~` (change to home directory)
- `mkdir`: Create a new directory.
    - `mkdir new_dir` (create `new_dir`)
    - `mkdir -p path/to/new_dir` (create nested directories)
- `rmdir`: Remove empty directories.
    - `rmdir dir` (remove `dir`)
    - `rmdir -p path/to/dir` (remove directories and their parents if empty)
- `rm`: Remove files or directories.
    - `rm file` (remove `file`)
    - `rm -r dir` (recursively remove `dir` and its contents)
    - `rm -f file` (force remove `file`)

### File Operations:

- `cp`: Copy files or directories.
    - `cp source destination` (copy `source` to `destination`)
    - `cp -r source_dir destination_dir` (recursively copy directories)
- `mv`: Move or rename files or directories.
    - `mv old_name new_name` (rename `old_name` to `new_name`)
    - `mv file1 file2 dir` (move `file1` and `file2` to `dir`)
- `touch`: Create an empty file or update file timestamps.
    - `touch file` (create `file`)
- `cat`: Concatenate and display file content.
    - `cat file` (display content of `file`)
- `head`: Display the beginning of a file.
    - `head file` (show the first 10 lines of `file`)
    - `head -n 20 file` (show the first 20 lines of `file`)
- `tail`: Display the end of a file.
    - `tail file` (show the last 10 lines of `file`)
    - `tail -n 20 file` (show the last 20 lines of `file`)

### 1. **File and Directory Management**

1. `ls`
2. `ls -l`
3. `ls -a`
4. `ls -lh`
5. `ls -R`
6. `pwd`
7. `cd /path/to/directory`
8. `cd ~`
9. `cd ..`
10. `cd -`
11. `mkdir directory_name`
12. `rmdir directory_name`
13. `rm filename`
14. `rm -r directory_name`
15. `rm -rf directory_name`
16. `cp source destination`
17. `cp -r source destination`
18. `mv source destination`
19. `mv old_name new_name`
20. `touch filename`
21. `stat filename`
22. `find /path -name "filename"`
23. `find /path -type f`
24. `find . -name "*.txt"`
25. `tree`
26. `ln filename link_name`
27. `ln -s filename symlink_name`
28. `which command`
29. `whereis command`
30. `updatedb`
31. `locate filename`
32. `file filename`
33. `chmod permissions filename`
34. `chmod +x filename`
35. `chmod 755 filename`
36. `chown user:group filename`
37. `chown -R user:group directory`
38. `chgrp group filename`
39. `umask`
40. `umask 022`
41. `readlink filename`
42. `realpath filename`
43. `basename filename`
44. `dirname filename`
45. `dir`
46. `dir -l`
47. `dircolors`
48. `lsblk`
49. `blkid`
50. `mount`
51. `umount`
52. `fstab`
53. `systemctl restart service`
54. `systemctl stop service`
55. `systemctl start service`
56. `systemctl enable service`
57. `systemctl disable service`
58. `xargs`
59. `install`
60. `mkfifo filename`
61. `read`
62. `wc`
63. `split`
64. `cmp`
65. `comm`
66. `cut`
67. `paste`
68. `tee`
69. `sponge`
70. `dir -p`
71. `find . -type f`
72. `find . -type d`
73. `find . -size +10M`
74. `find . -name "*.log"`
75. `find . -exec ls -lh {} \;`
76. `stat`
77. `tree -L 2`
78. `tree -d`
79. `tree -a`

### 2. **Text Viewing and Editing Commands**

80. `cat filename`
81. `more filename`
82. `less filename`
83. `head filename`
84. `head -n 10 filename`
85. `tail filename`
86. `tail -f filename`
87. `vim filename`
88. `vi filename`
89. `nano filename`
90. `gedit filename`
91. `emacs filename`
92. `nano -w filename`
93. `tee filename`
94. `cut -d ":" -f 1 filename`
95. `cut -f1,2 filename`
96. `sort filename`
97. `sort -r filename`
98. `uniq filename`
99. `wc filename`
100. `wc -l filename`
101. `wc -w filename`
102. `grep "pattern" filename`
103. `grep -i "pattern" filename`
104. `grep -r "pattern" /path`
105. `grep -v "pattern" filename`
106. `grep -E "regex" filename`
107. `sed 's/pattern/replacement/' filename`
108. `sed 's/pattern/replacement/g' filename`
109. `awk '{print $1}' filename`
110. `awk '{print $2, $3}' filename`
111. `tr 'a-z' 'A-Z' < input.txt`
112. `tr -d 'a' < input.txt`
113. `join file1 file2`
114. `diff file1 file2`
115. `cmp file1 file2`
116. `split filename`
117. `split -l 10 filename`
118. `emacs filename`
119. `vimdiff file1 file2`
120. `colordiff file1 file2`
121. `fold -w 80`
122. `shuf filename`
123. `uniq -c filename`
124. `fmt filename`
125. `column -t filename`

### 3. **System Information Commands**

126. `uname`
127. `uname -a`
128. `top`
129. `htop`
130. `ps`
131. `ps aux`
132. `ps -ef`
133. `df`
134. `df -h`
135. `du`
136. `du -sh *`
137. `free`
138. `free -h`
139. `uptime`
140. `who`
141. `whoami`
142. `w`
143. `id`
144. `last`
145. `last -n 10`
146. `dmesg`
147. `lscpu`
148. `lshw`
149. `lsblk`
150. `lsusb`
151. `lspci`
152. `ifconfig`
153. `ip addr show`
154. `ip a`
155. `ip link`
156. `hostname`
157. `hostnamectl`
158. `timedatectl`
159. `journalctl`
160. `systemctl status`
161. `systemctl list-units`
162. `sysctl -a`
163. `vmstat`
164. `iostat`
165. `mpstat`
166. `sar`
167. `watch command`
168. `uptime`
169. `arch`
170. `file /path/to/file`
171. `mount`
172. `umount`
173. `blkid`
174. `lvm`
175. `dmidecode`
176. `lsmod`
177. `modinfo`
178. `lsmod`
179. `lsusb`
180. `lsblk`
181. `ps -A`
182. `findmnt`
183. `ip route`

### 4. **Package Management Commands (Debian-based Systems)**

184. `sudo apt update`
185. `sudo apt upgrade`
186. `sudo apt install package_name`
187. `sudo apt remove package_name`
188. `sudo apt autoremove`
189. `sudo apt purge package_name`
190. `sudo apt-get install package_name`
191. `sudo apt-get remove package_name`
192. `sudo apt-get update`
193. `sudo apt-get upgrade`
194. `dpkg -l`
195. `dpkg -i package_name.deb`
196. `apt-cache search package_name`
197. `apt-cache show package_name`
198. `apt show package_name`
199. `apt list --installed`
200. `apt list package_name`
201. `sudo apt-get autoremove`
202. `sudo apt-get clean`
203. `sudo apt-get autoclean`
204. `sudo dpkg --configure -a`
205. `sudo apt-get dist-upgrade`
206. `apt list --upgradable`

### 5. **Package Management Commands (Red Hat-based Systems)** 

207. `sudo yum update`
208. `sudo yum install package_name`
209. `sudo yum remove package_name`
210. `sudo yum list installed`
211. `sudo yum search package_name`
212. `sudo yum info package_name`
213. `sudo yum clean all`
214. `sudo dnf install package_name`
215. `sudo dnf remove package_name`
216. `sudo dnf update`
217. `sudo dnf list installed`
218. `yum history`

### 6. **Disk Usage and Partitioning**

219. `fdisk -l`
220. `fdisk /dev/sda`
221. `parted /dev/sda`
222. `mkfs.ext4 /dev/sda1`
223. `tune2fs -l /dev/sda1`
224. `resize2fs /dev/sda1`
225. `mount /dev/sda1 /mnt`
226. `umount /mnt`
227. `lsblk`
228. `partprobe`
229. `gparted`
230. `df -h`
231. `du -sh *`
232. `smartctl -a /dev/sda`
233. `hdparm -I /dev/sda`
234. `mount -t ext4 /dev/sda1 /mnt`
235. `mount -t ntfs /dev/sda1 /mnt`
236. `swapoff -a`
237. `swapon -a`
238. `tune2fs -l /dev/sda1`
239. `fsck /dev/sda1`

### 7. **Networking Commands**

240. `ping 8.8.8.8`
241. `ping` [www.google.com](https://www.google.com "https://www.google.com/")
242. `traceroute google.com`
243. `nslookup google.com`
244. `dig google.com`
245. `ifconfig`
246. `ip addr`
247. `ip link`
248. `netstat`
249. `netstat -tuln`
250. `ss -tuln`
251. `route`
252. `route -n`
253. `wget` [http://example.com/file](http://example.com/file "http://example.com/file")
254. `curl` [http://example.com](http://example.com "http://example.com/")
255. `scp user@host:/path/to/file /local/path`
256. `rsync -avz source destination`
257. `ftp`
258. `sftp`
259. `telnet host port`
260. `ssh user@host`
261. `ssh -p port user@host`
262. `iptables -L`
263. `iptables -A INPUT -p tcp --dport 22 -j ACCEPT`
264. `ufw enable`
265. `ufw allow 22/tcp`
266. `ufw deny 23`
267. `ufw status`
268. `ufw reset`

### 8. **File Permissions and Ownership**

269. `chmod 755 filename`
270. `chmod +x filename`
271. `chmod -R 755 directory`
272. `chown user:group filename`
273. `chown -R user:group directory`
274. `chgrp group filename`
275. `umask 022`
276. `umask`
277. `setfacl`
278. `getfacl`
279. `ls -l`
280. `ls -Z`
281. `chcon`

### 9. **Process Management**

282. `ps aux`
283. `ps -ef`
284. `top`
285. `htop`
286. `kill <pid>`
287. `kill -9 <pid>`
288. `pkill process_name`
289. `killall process_name`
290. `bg`
291. `fg`
292. `jobs`
293. `nice`
294. `renice`
295. `at`
296. `cron`
297. `crontab -e`
298. `crontab -l`
299. `crontab -r`
300. `systemctl restart service`
301. `systemctl stop service`
302. `systemctl start service`
303. `systemctl status service`
304. `systemctl enable service`
305. `systemctl disable service`
306. `nice`
307. `renice`

### 10. **User and Group Management**

308. `useradd username`
309. `usermod -aG group username`
310. `userdel username`
311. `groupadd groupname`
312. `groupdel groupname`
313. `passwd username`
314. `chage -l username`
315. `chage -E 2024-12-31 username`
316. `id username`
317. `whoami`
318. `who`
319. `last`
320. `lastlog`
321. `adduser username`
322. `deluser username`
323. `groups username`
324. `sudo`
325. `sudo su`
326. `sudo usermod`
327. `sudo visudo`

### 11. **Searching and Finding**

328. `find /path -name "*.txt"`
329. `find /path -type f`
330. `find /path -mtime +5`
331. `locate filename`
332. `updatedb`
333. `grep -r "pattern" /path`
334. `grep "pattern" filename`
335. `grep -l "pattern" *`
336. `grep -i "pattern" filename`
337. `grep -v "pattern" filename`
338. `grep -E "regex" filename`

### 12. **Compression and Archiving**

339. `tar -cvf archive.tar directory`
340. `tar -xvf archive.tar`
341. `tar -czvf archive.tar.gz directory`
342. `tar -xzvf archive.tar.gz`
343. `tar -czf archive.tar.gz directory`
344. `tar -xzf archive.tar.gz`
345. `gzip filename`
346. `gunzip filename.gz`
347. `bzip2 filename`
348. `bunzip2 filename.bz2`
349. `xz filename`
350. `unxz filename.xz`
351. `zip archive.zip file1 file2`
352. `unzip archive.zip`
353. `rar a archive.rar file1 file2`
354. `unrar x archive.rar`

### 13. **Miscellaneous**

355. `history`
356. `history | grep command`
357. `clear`
358. `exit`
359. `echo "text"`
360. `echo $variable`
361. `date`
362. `cal`
363. `uptime`
364. `alias name='command'`
365. `unalias name`
366. `date +%Y-%m-%d`
367. `sleep 5`
368. `watch command`
369. `time command`
370. `man command`
371. `whatis command`
372. `info command`
373. `sudo command`
374. `sudo -i`
375. `sudo su`
376. `sudo visudo`
377. `sudo !!`
378. `sudo tee`
379. `sudo systemctl restart service`
380. `sudo shutdown now`
381. `sudo reboot`
382. `reboot`
383. `shutdown -h now`
384. `shutdown -r now`

### 14. **File System Management**

385. `mkfs.ext4 /dev/sda1`
386. `fsck /dev/sda1`
387. `mount /dev/sda1 /mnt`
388. `umount /mnt`
389. `tune2fs -l /dev/sda1`
390. `resize2fs /dev/sda1`
391. `e2fsck /dev/sda1`
392. `mount -o loop /path/to/file.iso /mnt`
393. `mount -t ntfs /dev/sda1 /mnt`
394. `mount -t ext4 /dev/sda1 /mnt`
395. `swapoff -a`
396. `swapon -a`

### 15. **Backup and Restore**

397. `rsync -avz source/ destination/`
398. `tar -cvf backup.tar directory/`
399. `tar -xvf backup.tar`
400. `cp -r source/ destination/`
401. `dd if=/dev/sda of=/path/to/backup.img`
402. `scp user@remote:/path/to/file /local/path`
403. `rsync -avz /local/backup/ remote:/path/`
404. `rsync -avz --delete /source/ /destination/`

### Linux Topics

### Basic File and Directory Commands

- `pwd` – Print the current working directory (shows where you are in the file system).
    - Example: `pwd`
- `cd` – Change the current directory.
    - Example: `cd /home/user/Documents`
- `ls` – List files and directories in the current directory.
    - Example: `ls`
- `mkdir` – Create a new directory.
    - Example: `mkdir new_folder`
- `rmdir` – Remove an empty directory.
    - Example: `rmdir old_folder`
- `rm` – Remove a file or directory.
    - Example: `rm file.txt`
    - To remove a directory with files: `rm -r folder_name`
- `cp` – Copy files or directories.
    - Example: `cp file1.txt file2.txt`
    - To copy a directory: `cp -r dir1/ dir2/`
- `mv` – Move or rename files and directories.
    - Example: `mv file1.txt newfile.txt` (rename)
    - To move a file: `mv file1.txt /home/user/Documents/`

### Text File Viewing and Editing

- `cat` – Display the content of a file.
    - Example: `cat file.txt`
- `more` – View the content of a file, one screen at a time.
    - Example: `more file.txt`
- `less` – Similar to `more`, but allows backward navigation.
    - Example: `less file.txt`
- `nano` – A simple text editor in the terminal.
    - Example: `nano file.txt`
    - Press `Ctrl + X` to exit.
- `echo` – Display a line of text or variable value.
    - Example: `echo "Hello, World!"`
- `head` – Show the first few lines of a file.
    - Example: `head file.txt`
- `tail` – Show the last few lines of a file.
    - Example: `tail file.txt`
- `wc` – Count words, lines, and characters in a file.
    - Example: `wc file.txt`

### System Information and Management

- `date` – Display the current system date and time.
    - Example: `date`
- `cal` – Display the current month's calendar.
    - Example: `cal`
- `whoami` – Show the current logged-in username.
    - Example: `whoami`
- `uptime` – Show how long the system has been running.
    - Example: `uptime`
- `hostname` – Display or set the system’s hostname.
    - Example: `hostname`
- `df` – Display disk space usage.
    - Example: `df -h`
- `free` – Display memory usage.
    - Example: `free -h`
- `top` – Display running processes and system resource usage.
    - Example: `top`

### User and Group Management

- `who` – Show who is logged into the system.
    - Example: `who`
- `whoami` – Show the current logged-in user.
    - Example: `whoami`
- `useradd` – Add a new user.
    - Example: `sudo useradd username`
- `passwd` – Change a user's password.
    - Example: `sudo passwd username`
- `groups` – Show the groups a user belongs to.
    - Example: `groups username`
- `id` – Display user ID (UID) and group ID (GID).
    - Example: `id username`

### File Permissions

- `chmod` – Change file permissions (read, write, execute).
    - Example: `chmod 755 file.txt` (Owner can read, write, and execute; group and others can read and execute)
- `chown` – Change file owner and group.
    - Example: `sudo chown user:group file.txt`
- `ls -l` – List files with detailed information (including permissions).
    - Example: `ls -l`

### Searching Files

- `find` – Search for files in a directory hierarchy.
    - Example: `find /home/user -name "*.txt"`
- `locate` – Find files by name quickly using a database (requires the `locate` database to be updated).
    - Example: `locate file.txt`
- `grep` – Search text in files for specific patterns.
    - Example: `grep "word" file.txt`

### Networking and Internet

- `ping` – Check the connectivity to a host or IP address.
    - Example: `ping google.com`
- `ifconfig` (or `ip a` on newer systems) – Display network interface information.
    - Example: `ifconfig`
- `curl` – Transfer data from or to a server using various protocols.
    - Example: `curl` [https://example.com](https://example.com "https://example.com/")
- `wget` – Download files from the web.
    - Example: `wget` [http://example.com/file.zip](http://example.com/file.zip "http://example.com/file.zip")

### Process Management

- `ps` – Display currently running processes.
    - Example: `ps aux`
- `kill` – Terminate a process by its PID (Process ID).
    - Example: `kill 1234` (where `1234` is the PID)
- `top` – Display system resource usage, running processes, and their statuses.
    - Example: `top`

### Disk and Filesystem Utilities

- `fdisk` – A tool for partitioning hard disks.
    - Example: `sudo fdisk -l` (list disk partitions)
- `mount` – Mount a filesystem.
    - Example: `sudo mount /dev/sda1 /mnt`
- `umount` – Unmount a mounted filesystem.
    - Example: `sudo umount /mnt`
- `lsblk` – List block devices and their mount points.
    - Example: `lsblk`
- `df` – Display disk space usage.
    - Example: `df -h`

### Package Management (Debian/Ubuntu-based systems)

- `apt-get update` – Update the package index.
    - Example: `sudo apt-get update`
- `apt-get upgrade` – Upgrade all installed packages to the latest versions.
    - Example: `sudo apt-get upgrade`
- `apt-get install` – Install a package.
    - Example: `sudo apt-get install firefox`
- `apt-get remove` – Remove a package.
    - Example: `sudo apt-get remove firefox`

### Archiving and Compression

- `tar` – Archive and compress files into a `.tar` file.
    - Example: `tar -cvf archive.tar file1 file2`
    - To extract: `tar -xvf archive.tar`
- `gzip` – Compress files with the `.gz` format.
    - Example: `gzip file.txt`
- `gunzip` – Decompress `.gz` files.
    - Example: `gunzip file.txt.gz`
- `zip` – Compress files into a `.zip` archive.
    - Example: `zip archive.zip file1 file2`
- `unzip` – Extract files from a `.zip` archive.
    - Example: `unzip archive.zip`

### Disk Usage and Management

- `du` – Display disk usage of files and directories.
    - Example: `du -sh folder_name`
- `lsblk` – List information about all block devices.
    - Example: `lsblk`
- `fsck` – Check and repair a filesystem.
    - Example: `sudo fsck /dev/sda1`

### System Shutdown and Reboot

- `shutdown` – Shut down the system.
    - Example: `sudo shutdown now`
- `reboot` – Reboot the system.
    - Example: `sudo reboot`
- `poweroff` – Turn off the system.
    - Example: `sudo poweroff`
### File and Directory Management

- `find` - Search for files in a directory hierarchy.
    - Example: `find /home/user -name "*.txt"`
- `locate` - Find files by name quickly using a database.
    - Example: `locate file.txt`
- `which` - Show the full path of shell commands.
    - Example: `which python`
- `basename` - Strips directory and suffix from filenames.
    - Example: `basename /path/to/file.txt`
- `dirname` - Get the directory name of a path.
    - Example: `dirname /path/to/file.txt`
- `ln` - Create hard and symbolic links.
    - Example: `ln -s /path/to/file /path/to/symlink`

### Text File Processing

- `grep` - Search for patterns in files.
    - Example: `grep "hello" file.txt`
- `awk` - A powerful text processing tool for pattern scanning and processing.
    - Example: `awk '{print $1}' file.txt`
- `sed` - Stream editor for transforming text.
    - Example: `sed 's/old/new/' file.txt`
- `tr` - Translate or delete characters.
    - Example: `echo "hello" | tr 'a-z' 'A-Z'`
- `tee` - Read from standard input and write to standard output and files.
    - Example: `echo "Hello World" | tee file.txt`

### System Monitoring and Performance

- `df -h` - Display disk space in a human-readable format.
- `du -sh` - Display directory space usage in a human-readable format.
- `free -m` - Display memory usage in megabytes.
- `iostat` - Report CPU and I/O statistics.
- `uptime` - Show how long the system has been running.
- `lscpu` - Display CPU architecture information.
- `dmesg` - Print kernel ring buffer messages.
- `lsof` - List open files and the processes using them.
- `tload` - Display terminal loading graph (in real-time).

### Networking

- `curl` - Transfer data from or to a server (supports many protocols).
    - Example: `curl` [http://example.com](http://example.com "http://example.com/")
- `wget` - Non-interactive network downloader.
    - Example: `wget` [http://example.com/file.zip](http://example.com/file.zip "http://example.com/file.zip")
- `ssh` - Secure Shell to login to a remote system.
    - Example: `ssh user@hostname`
- `scp` - Securely copy files between hosts over SSH.
    - Example: `scp file.txt user@hostname:/path/to/destination`
- `netstat` - Display network connections, routing tables, and interface statistics.
- `ss` - A utility to investigate sockets (faster than `netstat`).
- `traceroute` - Trace the route packets take to a network host.
    - Example: `traceroute google.com`
- `ifconfig` (or `ip a` on modern systems) - Display or configure network interfaces.
- `nslookup` - Query DNS records.
    - Example: `nslookup example.com`

### File Permissions and Ownership

- `chmod` - Change file permissions.
    - Example: `chmod 755 file.txt`
- `chown` - Change file owner and group.
    - Example: `chown user:group file.txt`
- `chgrp` - Change group ownership of a file.
    - Example: `chgrp group file.txt`
- `umask` - Set default file creation permissions.
    - Example: `umask 022`
- `getfacl` - Get file access control lists.
- `setfacl` - Set file access control lists.

### User Management

- `adduser` / `useradd` - Add a new user.
    - Example: `sudo useradd newuser`
- `passwd` - Change a user's password.
    - Example: `sudo passwd newuser`
- `usermod` - Modify a user account.
    - Example: `sudo usermod -aG group newuser`
- `deluser` / `userdel` - Delete a user account.
    - Example: `sudo userdel newuser`
- `groups` - Show user groups.
    - Example: `groups newuser`
- `who` - Display who is logged into the system.
- `w` - Show who is logged in and what they are doing.
- `last` - Show last login information.
- `sudo` - Run a command as a superuser or another user.

### Disk and Storage Management

- `fdisk` - Partition table manipulator for Linux.
    - Example: `sudo fdisk /dev/sda`
- `mkfs` - Create a filesystem on a device.
    - Example: `sudo mkfs.ext4 /dev/sda1`
- `mount` - Mount a filesystem.
    - Example: `sudo mount /dev/sda1 /mnt`
- `umount` - Unmount a filesystem.
    - Example: `sudo umount /mnt`
- `lsblk` - List information about block devices.
- `parted` - A tool for managing partitions.
- `blkid` - Find block device attributes.

### Process Management

- `ps` - List current running processes.
    - Example: `ps aux`
- `top` - Display tasks and their resource usage interactively.
- `htop` - An interactive process viewer, more user-friendly than `top`.
- `kill` - Terminate a process by PID.
    - Example: `kill 1234`
- `killall` - Kill processes by name.
    - Example: `killall processname`
- `bg` - Resume a suspended job in the background.
- `fg` - Bring a background job to the foreground.
- `jobs` - List background jobs.

### Archiving and Compression

- `tar` - Archive files.
    - Example: `tar -czvf archive.tar.gz file1 file2`
- `zip` - Compress files into a ZIP archive.
    - Example: `zip archive.zip file1 file2`
- `unzip` - Extract files from a ZIP archive.
    - Example: `unzip archive.zip`
- `gzip` - Compress files.
    - Example: `gzip file.txt`
- `gunzip` - Decompress files.
    - Example: `gunzip file.txt.gz`
- `bzip2` - Compress files (better compression than `gzip`).
    - Example: `bzip2 file.txt`
- `tar -xjvf` - Extract a `.tar.bz2` archive.

### System Administration and Maintenance

- `cron` - Daemon to execute scheduled commands.
- `crontab` - Edit cron jobs.
    - Example: `crontab -e`
- `systemctl` - Control the systemd system and service manager.
    - Example: `sudo systemctl restart nginx`
- `service` - Manage services on older systems (not using systemd).
    - Example: `sudo service apache2 restart`
- `journalctl` - Query and display logs from systemd.
    - Example: `journalctl -u nginx`
- `lsmod` - Show currently loaded kernel modules.
- `modprobe` - Add or remove modules from the Linux kernel.
- `lspci` - Display information about PCI buses and devices.
- `lsusb` - Display information about USB devices.
- `uname -r` - Show the kernel version.
- `hostname` - Show or set the system hostname.

### Disk and Filesystem Utilities

- `fsck` - Check and repair filesystem inconsistencies.
- `mount` - Mount a filesystem.
    - Example: `sudo mount /dev/sda1 /mnt`
- `df -h` - Display disk space usage in human-readable form.
- `du -sh` - Show the disk usage of files and directories.
- `xfs_check` - Check an XFS filesystem.
- `tune2fs` - Adjust tunable filesystem parameters for ext filesystems.

### Backup and Restore

- `rsync` - Sync files and directories between two locations.
    - Example: `rsync -av source/ destination/`
- `tar` - Archive files for backup.
    - Example: `tar -czvf backup.tar.gz /path/to/files`
