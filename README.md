# Role Name: elimina_snapshot

## 📌 Descripción

Este rol permite eliminar snapshots antiguos de máquinas virtuales en VMware vSphere.
Se basa en criterios de antigüedad e información obtenida directamente desde vCenter o ESXi.

Diseñado siguiendo las buenas prácticas recomendadas por Red Hat para roles reutilizables, mantenibles y documentados.

---

## ✅ Requerimientos del sistema / Control Node

- **Ansible** 2.12 o superior
- Acceso al entorno VMware vSphere/vCenter
- Python y librerías necesarias para las colecciones VMware
- Credenciales válidas para autenticación

---

## ✅ Colecciones utilizadas

Este rol utiliza los siguientes módulos de las colecciones `community.vmware` y `ansible.builtin`:

- `community.vmware.vmware_vm_info`
- `community.vmware.vmware_guest_info`
- `community.vmware.vmware_guest_snapshot`
- `ansible.builtin.include_tasks`
- `ansible.builtin.set_fact`

Si aún no tienes instaladas las colecciones necesarias:

```bash
ansible-galaxy collection install community.vmware
```

---
## Derechos de autor

Este rol es propiedad de **GBM**.
Su uso, copia o distribución está sujeto a autorización previa por parte de la empresa.
