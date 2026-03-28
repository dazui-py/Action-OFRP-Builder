# Compilar Recovery via GitHub Actions

- Suporte para OrangeFox. Para TWRP e outros derivados, use o [Action-TWRP-Builder](https://github.com/azwhikaru/Action-TWRP-Builder).

---

## Agradecimentos
- Todos os contribuidores

---

## Notas de Atualização

= 20/04/2023
 * Primeira versão funcional enviada.

-----

## Descrição dos Parâmetros

| Parâmetro | Descrição | Exemplo |
| :--- | :--- | :--- |
| `SYNC_URL` | Script de sincronização do OrangeFox | https://gitlab.com/OrangeFox/sync.git |
| `MANIFEST_BRANCH` | Branch do código-fonte (Source) | 12.1 |
| `DEVICE_TREE_URL` | URL da Device Tree | https://github.com/OrangeFoxRecovery/device_xiaomi_laurel_sprout |
| `DEVICE_TREE_BRANCH` | Branch da Device Tree | fox_12.1 |
| `DEVICE_PATH` | Caminho da Device Tree | device/xiaomi/laurel_sprout |
| `COMMON_TREE_URL` | URL da Common Tree | |
| `COMMON_PATH` | Caminho da Common Tree | |
| `DEVICE_NAME` | Codename do modelo | laurel_sprout |
| `MAKEFILE_NAME` | Nome da Makefile | twrp_laurel_sprout |
| `BUILD_TARGET` | Partição de destino (boot/recovery/vendorboot) | recovery |

-----

## Como usar

Exemplo: se o seu usuário do GitHub for "JohnSmith"
#### 1. Clique no botão "Fork" no canto superior direito deste repositório
![image](https://user-images.githubusercontent.com/37921907/177914706-c92476c5-7e14-4fb3-be94-0c8a11dae874.png)

#### 2. Aguarde o redirecionamento automático; você verá o seu próprio nome de usuário
![image](https://user-images.githubusercontent.com/37921907/177915106-5bde6fc9-303c-479e-b290-22b48efd1e4e.png)

-----

## Iniciando a Compilação da Recovery
#### 9. Vá para "Actions" -> "Recovery Build"
![image](https://user-images.githubusercontent.com/37921907/177915304-8731ed80-1d49-48c9-9848-70d0ac8f2720.png)

#### 10. Clique em "Run workflow" e preencha conforme a "Descrição dos Parâmetros" acima
![image](https://user-images.githubusercontent.com/37921907/177915346-71c29149-78fb-4a00-996f-5d84ffc9eb8c.png)

#### 11. Após preencher, clique em "Run workflow" para iniciar a execução

-----

## Resultados da Compilação
Os arquivos podem ser baixados em [Releases](../../releases).

> **O arquivo não foi enviado para a Release?** > Verifique a etapa "Check the output directory before uploading" nos logs e confira se o nome do arquivo gerado corresponde ao esperado.
