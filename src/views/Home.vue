<template>
  <div class="home">
    <section>
      <header>Tabelas</header>

      <div class="data-grid">
        <header class="data-grid__header">
          <div class="data-grid__button-group">
            <button class="data-grid__button">
              <span class="icon"><i class="fas fa-plus"></i></span>
              Novo
            </button>

            <button class="data-grid__button">
              <span class="icon"><i class="far fa-edit"></i></span>
              Editar
            </button>

            <button class="data-grid__button">
              <span class="icon"><i class="far fa-trash-alt"></i></span>
              Remover
            </button>

            <div class="data-grid__dropdown">
              <button class="data-grid__dropdown__toggle data-grid__button">
                <span class="icon icon-leading"><i class="far fa-copy"></i></span>
                <span class="data-grid__dropdown__toggle__text">Transportar</span>
                <span class="icon icon-trailing"><i class="fas fa-chevron-down"></i></span>
              </button>

              <div class="data-grid__dropdown__content">
                <div class="data-grid__dropdown__item">Item 1</div>
                <div class="data-grid__dropdown__item">Item 2</div>
                <div class="data-grid__dropdown__item">Item 3</div>
                <div class="data-grid__dropdown__item">Item 4</div>
                <div class="data-grid__dropdown__item">Item 5</div>
              </div>
            </div>
          </div>

          <div class="data-grid__filters">
            <select class="data-grid__filters__input-control">
              <option value="Item1">Item 1</option>
              <option value="Item2">Item 2</option>
              <option value="Item3">Item 3</option>
              <option value="Item4">Item 4</option>
            </select>

            <select class="data-grid__filters__input-control">
              <option value="Item1">Item 1</option>
              <option value="Item2">Item 2</option>
              <option value="Item3">Item 3</option>
              <option value="Item4">Item 4</option>
            </select>

            <select class="data-grid__filters__input-control">
              <option value="Item1">Item 1</option>
              <option value="Item2">Item 2</option>
              <option value="Item3">Item 3</option>
              <option value="Item4">Item 4</option>
            </select>
          </div>
        </header>
        
        <table class="data-grid__table">
          <thead>
            <tr>
              <th>Tipo</th>
              <th>Folha</th>
              <th>Título</th>
              <th>Pessoa Jurídica</th>
            </tr>
          </thead>

          <tbody>
            <tr v-for="item in items" :key="item.id">
              <td>{{ item.tipo }}</td>
              <td>{{ item.folha }}</td>
              <td>{{ item.titulo }}</td>
              <td>{{ item.pessoa_juridica }}</td>
            </tr>
          </tbody>
        </table>

        <div class="data-grid__footer">
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'Home',

  mounted() {
    const dropdowns = document.querySelectorAll('.data-grid__dropdown')

    dropdowns.forEach(dropdown => {
      const toggle = dropdown.querySelector('.data-grid__dropdown__toggle')

      toggle.addEventListener('click', () => {
        dropdown.classList.toggle('data-grid__dropdown--show-content')
      })

      document.addEventListener('click', event => {
        if (!dropdown.contains(event.target)) {
          dropdown.classList.remove('data-grid__dropdown--show-content')
        }
      })
    })
  },

  data() {
    return {
      items: [
        {
          id: 1,
          tipo: 'Consignação',
          folha: 'Folha normal',
          titulo: 'ADPETO - Juntos Contra a Fome - Reg. Próprio',
          pessoa_juridica: 'ADPETO'
        },
        {
          id: 2,
          tipo: 'Consignação',
          folha: 'Folha normal',
          titulo: 'ADPETO - Juntos Contra a Fome - Reg. Próprio',
          pessoa_juridica: 'ADPETO'
        },
        {
          id: 3,
          tipo: 'Consignação',
          folha: 'Folha normal',
          titulo: 'ADPETO - Juntos Contra a Fome - Reg. Próprio',
          pessoa_juridica: 'ADPETO'
        },
        {
          id: 4,
          tipo: 'Consignação',
          folha: 'Folha normal',
          titulo: 'ADPETO - Juntos Contra a Fome - Reg. Próprio',
          pessoa_juridica: 'ADPETO'
        },
        {
          id: 5,
          tipo: 'Consignação',
          folha: 'Folha normal',
          titulo: 'ADPETO - Juntos Contra a Fome - Reg. Próprio',
          pessoa_juridica: 'ADPETO'
        },
        {
          id: 6,
          tipo: 'Consignação',
          folha: 'Folha normal',
          titulo: 'ADPETO - Juntos Contra a Fome - Reg. Próprio',
          pessoa_juridica: 'ADPETO'
        },
        {
          id: 7,
          tipo: 'Consignação',
          folha: 'Folha normal',
          titulo: 'ADPETO - Juntos Contra a Fome - Reg. Próprio',
          pessoa_juridica: 'ADPETO'
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
section {
  & > header {
    font-size: 1.5rem;
    margin: 1rem 0;
  }
}

.data-grid {
  border: 1px solid #112CD3;
  font-size: .85rem;
  overflow-x: auto;

  &__header {
    display: flex;
  }

  &__button-group {
    display: flex;
    align-items: center;
    flex-wrap: nowrap;

    .data-grid__button {
      border-top: 0;
      border-left: 0;
      border-radius: 0;
    }
  }

  &__button {
    border: 1px solid #112CD3;
    background-color: white;
    border-radius: 4px;
    color: #112CD3;
    padding: .35rem 1rem;
    outline: none;
    transition: .3s;

    &:hover {
      background-color: #112CD3;
      color: white;
      cursor: pointer;
    }
  }

  &__dropdown {
    display: inline-block;
    position: relative;

    .icon-leading {
      margin-right: .3rem;
    }

    .icon-trailing {
      font-size: .75rem;
      margin-left: .5rem;
    }

    &__content {
      display: none;
      background-color: white;
      box-shadow: 0 1px 1px rgba(0, 0, 0, 0.11), 
                  0 2px 2px rgba(0, 0, 0, 0.11), 
                  0 4px 4px rgba(0, 0, 0, 0.11), 
                  0 6px 8px rgba(0, 0, 0, 0.11),
                  0 8px 16px rgba(0, 0, 0, 0.11);
      position: absolute;
      top: 100%;
      right: 0;
      width: 15rem;
      padding: .75rem;
    }

    &__item {
      border-radius: 4px;
      padding: .5rem 1rem;
      transition: .3s;

      &:hover {
        background-color: rgba(0, 0, 0, 0.05);
        cursor: pointer;
      }
    }

    &--show-content &__content {
      display: block;
    }
  }

  &__filters {
    display: flex;
    flex-wrap: nowrap;
    margin-left: auto;

    &__input-control {
      border: 1px solid #112CD3;
      border-top: 0;
      background-color: white;
      // border-radius: 4px;
      cursor: pointer;
      height: 100%;
      padding: .35rem 1rem;
      outline: none;
      transition: .3s;
    }

    &__input-control:not(:last-child) {
      margin-right: .5rem;
    }

    &__input-control:last-child {
      border-right: 0;
    }
  }

  .table-responsive {
    width: 100%;
    overflow: auto;
  }

  &__table {
    border-collapse: collapse;
    width: 100%;
  }

  &__table, &__table th, &__table td {
    border: 1px solid #ddd;
  }

  &__table th, &__table td {
    padding: .35rem .75rem;
    text-align: left;
  }

  &__table tbody {
    tr, tr.active {
      &:hover {
        background-color: #efefef;
      }
    }
  }
}
</style>