# 🌿 EcoFood — Sistema de Controle de Desperdício Alimentar Escolar

Sistema web em Django para monitorar, registrar e reduzir o desperdício alimentar em escolas.

---

## ✨ Funcionalidades

- **Dashboard** com KPIs em tempo real (desperdício, refeições, alertas de estoque)
- **Gráfico de evolução mensal** do desperdício (últimos 6 meses)
- **Ranking** dos alimentos mais desperdiçados
- **Gestão de Alimentos** com cálculo automático de desperdício e % de consumo
- **Registro de Desperdícios** com motivos categorizados e filtros por período
- **Controle de Refeições** com alimentos, comensais e responsável
- **Gestão de Estoque** com alertas de quantidade mínima e validade
- **Cadastro de Fornecedores**
- **Relatórios** por tipo e período
- **Autenticação** com login/logout

---

## 🚀 Como rodar

### 1. Pré-requisitos
```bash
python -m pip install -r requirements.txt
```

### 2. Banco de dados
```bash
python manage.py makemigrations
python manage.py migrate
```

### 3. Criar superusuário (admin)
```bash
python manage.py createsuperuser
```

### 4. Rodar o servidor
```bash
python manage.py runserver
```

Acesse: **http://127.0.0.1:8000**

---

## 📁 Estrutura do projeto

```
ecofood/
├── config/
│   ├── settings.py       # Configurações Django
│   └── urls.py           # URLs raiz
├── app/
│   ├── models.py         # Modelos do banco
│   ├── views.py          # Views e lógica
│   ├── forms.py          # Formulários
│   ├── urls.py           # URLs da app
│   ├── admin.py          # Admin configurado
│   ├── templates/app/    # Templates HTML
│   │   ├── base.html
│   │   ├── login.html
│   │   ├── dashboard.html
│   │   ├── alimentos.html
│   │   ├── desperdicios.html
│   │   ├── refeicoes.html
│   │   ├── estoque.html
│   │   ├── fornecedores.html
│   │   ├── relatorios.html
│   │   ├── form_generic.html
│   │   └── confirm_delete.html
│   └── static/app/css/
│       └── main.css      # Design system completo
├── manage.py
└── requirements.txt
```

---

## 🎨 Design

- **Paleta**: Verde floresta profundo + âmbar quente
- **Tipografia**: Instrument Serif (títulos) + Inter (corpo)
- **Assinatura**: Indicador folha orgânica na barra lateral + cards com formas orgânicas
- **Responsivo**: Mobile-first com sidebar adaptável

---

## 🔑 Admin Django

Acesse `/admin/` para gerenciar todos os dados diretamente.
