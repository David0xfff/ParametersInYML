# Azure DevOps Pipeline - Uso de Parámetros

Este pipeline YAML en Azure DevOps demuestra cómo utilizar **parámetros** para personalizar valores como nombres de etapas, nombres de jobs, cadenas de texto y números. Es útil cuando se requiere reusar lógica o cambiar valores dinámicamente sin duplicar código.

---

## 🎛️ Parámetros Definidos

```yaml
parameters:
- name: myStage
  type: string
  default: 'Etapas (Stage)'

- name: myJob
  type: string
  default: 'Job1'

- name: myString
  type: string
  default: 'Valor por defecto'

- name: mynum
  displayName: 'My numero de parametro'
  type: number
  default: 123
