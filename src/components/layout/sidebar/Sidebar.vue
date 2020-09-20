<template>
  <div class="sidebar">
    <nav class="nav" ref="nav">
      <a href="#" class="item" data-target="#controle-almoxarifado" title="Controle Almoxarifado">
        <span class="icon icon-leading"><i class="fas fa-dolly-flatbed"></i></span>
        <span class="item__text">Controle Almoxarifado</span>
        <span class="icon icon-trailing"></span>
      </a>

      <a href="#" class="item" data-target="#controle-patrimonial" title="Controle Patrimonial">
        <span class="icon icon-leading"><i class="fas fa-house-user"></i></span>
        <span class="item__text">Controle Patrimonial</span>
        <span class="icon icon-trailing"></span>
      </a>

      <a href="#" class="item" title="Diárias" data-target="#diarias">
        <span class="icon icon-leading"><i class="fas fa-comment-dollar"></i></span>
        <span class="item__text">Diárias</span>
        <span class="icon icon-trailing"></span>
      </a>

      <a href="#" class="item" title="EDOC" data-target="#edoc">
        <span class="icon icon-leading"><i class="fas fa-atlas"></i></span>
        <span class="item__text">EDOC</span>
        <span class="icon icon-trailing"></span>
      </a>

      <a href="#" class="item" title="Financeiro" data-target="#financeiro">
        <span class="icon icon-leading"><i class="fas fa-dollar-sign"></i></span>
        <span class="item__text">Financeiro</span>
        <span class="icon icon-trailing"></span>
      </a>

      <a href="#" class="item" title="Folha de Pagamento" data-target="#folha-de-pagamento">
        <span class="icon icon-leading"><i class="fas fa-hand-holding-usd"></i></span>
        <span class="item__text">Folha de Pagamento</span>
        <span class="icon icon-trailing"></span>
      </a>

      <a href="#" class="item" title="Gestão de Pessoas" data-target="#gestao-de-pessoas">
        <span class="icon icon-leading"><i class="fas fa-smile"></i></span>
        <span class="item__text">Gestão de Pessoas</span>
        <span class="icon icon-trailing"></span>
      </a>

      <a href="#" class="item" title="Indenizações">
        <span class="icon icon-leading"><i class="fas fa-money-check-alt"></i></span>
        <span class="item__text">Indenizações</span>
        <span class="icon icon-trailing"></span>
      </a>

      <a href="#" class="item" title="Painel de Controle">
        <span class="icon icon-leading"><i class="fas fa-cogs"></i></span>
        <span class="item__text">Painel de Controle</span>
        <span class="icon icon-trailing"></span>
      </a>

      <a href="#" class="item" title="Portal do Servidor">
        <span class="icon icon-leading"><i class="fas fa-id-card-alt"></i></span>
        <span class="item__text">Portal do Servidor</span>
        <span class="icon icon-trailing"></span>
      </a>

      <a href="#" class="item" title="Recursos Humanos">
        <span class="icon icon-leading"><i class="fas fa-users"></i></span>
        <span class="item__text">Recursos Humanos</span>
        <span class="icon icon-trailing"></span>
      </a>

      <a href="#" class="item" title="Subdefensoria">
        <span class="icon icon-leading"><i class="fas fa-store-alt"></i></span>
        <span class="item__text">Subdefensoria</span>
        <span class="icon icon-trailing"></span>
      </a>

      <div class="nav-end">
        <a href="#" class="item" title="Configurações">
          <span class="icon icon-leading"><i class="fas fa-cog"></i></span>
          <span class="item__text">Configurações</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item" title="Ajuda">
          <span class="icon icon-leading"><i class="fas fa-question-circle"></i></span>
          <span class="item__text">Ajuda</span>
          <span class="icon icon-trailing"></span>
        </a>

        <div class="divider"></div>

        <a href="#" class="item toggle-nav" ref="toggle-nav" title="Expandir">
          <span class="icon icon-leading"><i class="fas fa-expand"></i></span>
        </a>
      </div>
    </nav>

    <nav class="subnav" ref="subnav">
      <div class="subnav__nav" id="controle-almoxarifado">
        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Relatórios</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-sliders-h"></i></span>
          <span class="item__text">Configurações</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-file-invoice-dollar"></i></span>
          <span class="item__text">Gestor de Solicitações</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-list-ol"></i></span>
          <span class="item__text">Gestão Almoxarifado</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="far fa-money-bill-alt"></i></span>
          <span class="item__text">Grupo Espécie</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-globe-americas"></i></span>
          <span class="item__text">Solicitação</span>
          <span class="icon icon-trailing"></span>
        </a>
      </div>

      <div class="subnav__nav" id="controle-patrimonial">
        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Relatórios</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-laptop-house"></i></span>
          <span class="item__text">Avaliação Patrimonial</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-sliders-h"></i></span>
          <span class="item__text">Configurações</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-file-invoice-dollar"></i></span>
          <span class="item__text">Contas Patrimoniais</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-list-ol"></i></span>
          <span class="item__text">Gestor de Inventários</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="far fa-money-bill-alt"></i></span>
          <span class="item__text">Grupo Espécie</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-globe-americas"></i></span>
          <span class="item__text">Localizações Patrimoniais</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-sort-amount-down"></i></span>
          <span class="item__text">Sequência Patrimonial</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-tasks"></i></span>
          <span class="item__text">Tabela de Avaliação</span>
          <span class="icon icon-trailing"></span>
        </a>
      </div>

      <div class="subnav__nav" id="diarias">
        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Relatórios</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-laptop-house"></i></span>
          <span class="item__text">Agenda de Viagens</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-sliders-h"></i></span>
          <span class="item__text">Avaliar Prestação de Contas</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-file-invoice-dollar"></i></span>
          <span class="item__text">Configurações</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-list-ol"></i></span>
          <span class="item__text">Gestor de Bilhetes Aéreos</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="far fa-money-bill-alt"></i></span>
          <span class="item__text">Gestor de Devoluções</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-globe-americas"></i></span>
          <span class="item__text">Gestor de Itinerários</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-sort-amount-down"></i></span>
          <span class="item__text">Gestor de Pagamentos</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-tasks"></i></span>
          <span class="item__text">Gestor de Diárias</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="far fa-money-bill-alt"></i></span>
          <span class="item__text">Gestor de Diárias - Administrativo</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="far fa-money-bill-alt"></i></span>
          <span class="item__text">Justificativas</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="far fa-money-bill-alt"></i></span>
          <span class="item__text">Pré-análise</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="far fa-money-bill-alt"></i></span>
          <span class="item__text">Tabela de diárias e cargos</span>
          <span class="icon icon-trailing"></span>
        </a>
      </div>

      <div class="subnav__nav" id="edoc">
        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Funcionalidades</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-laptop-house"></i></span>
          <span class="item__text">Relatórios</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-sliders-h"></i></span>
          <span class="item__text">Caixa de Entrada</span>
          <span class="icon icon-trailing"></span>
        </a>
      </div>

      <div class="subnav__nav" id="financeiro">
        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Folha de Pagamento</span>
          <span class="icon icon-trailing"></span>
        </a>
      </div>

      <div class="subnav__nav" id="folha-de-pagamento">
        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Imposto de Renda</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Parâmetros</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Plan Saúde</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Previdências</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Relatório</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Salários</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Viabilize</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Auditoria - Contracheques</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Configuração</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Controlador</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Gerenciador de Pensões</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Importador de lançamentos</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Lançador</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Terço de Férias</span>
          <span class="icon icon-trailing"></span>
        </a>
      </div>

      <div class="subnav__nav" id="gestao-de-pessoas">
        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Capacitações</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Relatórios</span>
          <span class="icon icon-trailing"></span>
        </a>

        <a href="#" class="item">
          <span class="icon icon-leading"><i class="fas fa-scroll"></i></span>
          <span class="item__text">Gerenciador de Capacitações</span>
          <span class="icon icon-trailing"></span>
        </a>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Sidebar',

  mounted() {
    this.configureToogleNav()
    this.configureNav()
  },

  methods: {
    configureToogleNav() {
      const nav = this.$refs['nav']
      const toggleNav = this.$refs['toggle-nav']
      
      toggleNav.addEventListener('click', () => {
        nav.classList.toggle('nav--expand')
      })
    },

    configureNav() {
      const nav = this.$refs['nav']
      const subnav = this.$refs['subnav']
      const items = nav.querySelectorAll('.item')

      items.forEach(item => {
        item.addEventListener('click', () => {
          const itemTarget = item.dataset.target

          if (itemTarget != null) {
            subnav.classList.add('subnav--active')

            document.querySelectorAll('.item--active').forEach(itemActive => {
              itemActive.classList.remove('item--active')
            })

            item.classList.add('item--active')

            const elementsTargetOpened = document.querySelectorAll('.subnav__nav--show')
            elementsTargetOpened.forEach(item => {
              item.classList.remove('subnav__nav--show')
            })

            const elementTarget = document.querySelector(itemTarget)
            elementTarget.classList.add('subnav__nav--show')
          }
        })
      })
    }
  }
}
</script>

<style lang="scss" scoped>
.sidebar, .nav, .subnav {
  height: 100%;
}

.sidebar {
  position: fixed;
  top: 0;
  left: 0;
  display: flex;
}

.nav {
  background-color: #112CD3;
  display: flex;
  flex-direction: column;
  overflow: auto;
  transition: width .3s cubic-bezier(0.165, 0.84, 0.44, 1);
  width: calc(2 * 1rem + 2rem);
}

.nav--expand {
  width: 15rem;
}

.nav-end {
  margin-top: auto;
}

.subnav {
  background-color: #040609;
}

.subnav--active {
  width: 20rem;
}

.subnav .subnav__nav {
  display: none;
}

.subnav .subnav__nav.subnav__nav--show {
  display: block;
}

.item {
  color: white;
  display: block;
  padding: .65rem 1rem;
  text-decoration: none;
  transition: .3s;
  white-space: nowrap;

  .icon.icon-leading {
    display: inline-block;
    font-size: 1.25rem;
    margin-right: 1rem;
    text-align: center;
    width: 2rem;
  }

  &:not(.toggle-nav):hover, &--active {
    background-color: #040609;
  }
}

.subnav .item {
  color: #999;

  &:hover {
    background-color: white;
    color: #333;
  }
}

.divider {
  height: 1px;
  background-color: rgba(0, 0, 0, .25);
}
</style>
