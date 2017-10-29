class: center, middle

# 容器网络

&nbsp;
&nbsp;

#### 崔治丞   

主页: https://github.com/CuiZhicheng/slidedemo

---

## 本讲内容

### 1. 容器网络

### 2. CNI与CNM

#### &nbsp; &nbsp; 2.1 CNM
#### &nbsp; &nbsp; 2.2 CNI
#### &nbsp; &nbsp; 2.3 对比

---

## 容器网络

### 容器的特点

#### &nbsp; &nbsp; 轻量级
#### &nbsp; &nbsp; 生命周期短
#### &nbsp; &nbsp; 数量多

---

## 容器网络

### 容器网络 VS 虚拟机网络

#### &nbsp; &nbsp; 1. 虚拟机隔离机制好，虚拟机网卡几乎等同于硬件网卡；容器只是通过namespace在内核中进行隔离，安全性不如虚拟机；
#### &nbsp; &nbsp; 2. 针对安全问题，容器在公有环境下，多部署在虚拟机内部，网络形成多重嵌套；
#### &nbsp; &nbsp; 3. 容器的部署可能在同一物理、虚拟机上，也可能分布在不同机器上；
#### &nbsp; &nbsp; 4. 容器生命周期短，迁移快，网络策略更新及IP管理（IPAM）需要高效；
#### &nbsp; &nbsp; 5. 容器数量很多，多个机器间可能会产生ARP Flooding。

### 容器与应用绑定，不同应用会产生不同场景，需要针对不同的需求制定网络方案。

---

```c
int main()
{
  printf("Hello world\n");
  return 0 ;
}
```

---

## 插图

** Ada Lovelace **

<img src="https://upload.wikimedia.org/wikipedia/commons/9/95/Ada_Lovelace_color.svg" width=300 style="margin: 0px 80px">

---

## `\(\LaTeX{}\)` in remark


1. This is an inline integral: `\(\int_a^bf(x)dx\)`
2. More `\(x={a \over b}\)` formulae.

Display formula:

$$e^{i\pi} + 1 = 0$$

---

class: center, middle

# 谢谢
