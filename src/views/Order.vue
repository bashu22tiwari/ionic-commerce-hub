<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-back-button default-href="/" slot="start" />
        <ion-title>{{ $t("Orders") }}</ion-title>
        <ion-buttons slot="end">
          <ion-button fill="clear">
            <ion-icon slot="icon-only" :icon="syncOutline" />
          </ion-button>
          <ion-button fill="clear">
            <ion-icon slot="icon-only" :icon="downloadOutline" />
          </ion-button>
          <ion-button fill="clear" class="mobile-only">
            <ion-icon slot="icon-only" :icon="filterOutline" />
          </ion-button>
        </ion-buttons>
      </ion-toolbar>
    </ion-header>

    <ion-content>
      <div class="find">
        <section class="search">
          <ion-searchbar />
        </section>

        <aside class="filters desktop-only">
          <ion-list>
            <ion-list-header>Date</ion-list-header>
            <ion-item>
              <ion-label>order created</ion-label>
              <ion-select value="any">
                <ion-select-option value="any">any</ion-select-option>
              </ion-select>
            </ion-item>
            <ion-item>
              <ion-label>order created</ion-label>
              <ion-select value="any">
                <ion-select-option value="any">any</ion-select-option>
              </ion-select>
            </ion-item>
            <ion-item>
              <ion-label>order created</ion-label>
              <ion-select value="any">
                <ion-select-option value="any">any</ion-select-option>
              </ion-select>
            </ion-item>
          </ion-list>
          <ion-list>
            <ion-list-header>Type</ion-list-header>
            <ion-item>
              <ion-label>order created</ion-label>
              <ion-checkbox />
            </ion-item>
            <ion-item>
              <ion-label>order created</ion-label>
              <ion-checkbox />
            </ion-item>
            <ion-item>
              <ion-label>order created</ion-label>
              <ion-checkbox />
            </ion-item>
          </ion-list>
          <ion-list>
            <ion-list-header>Date</ion-list-header>
            <ion-item>
              <ion-label>order created</ion-label>
              <ion-select value="any">
                <ion-select-option value="any">any</ion-select-option>
              </ion-select>
            </ion-item>
            <ion-item>
              <ion-label>order created</ion-label>
              <ion-select value="any">
                <ion-select-option value="any">any</ion-select-option>
              </ion-select>
            </ion-item>
            <ion-item>
              <ion-label>order created</ion-label>
              <ion-select value="any">
                <ion-select-option value="any">any</ion-select-option>
              </ion-select>
            </ion-item>
          </ion-list>

          <ion-card>
            <ion-toolbar>
              <ion-title>Purchase date</ion-title>
            </ion-toolbar>
            <ion-card-content>
              <ion-chip>
                <ion-label>PO #</ion-label>
              </ion-chip>
              <ion-chip>
                <ion-label>PO #</ion-label>
              </ion-chip>
            </ion-card-content>
          </ion-card>
        </aside>

        <main class="main">
          <section class="sort"></section>

           <hr />

          <section class="section-header">
            <div class="primary-info">
               <ion-item lines="none">
                <ion-label>
                  Order ID
                  <p>Customer Name</p>
                </ion-label>
              </ion-item>
            </div>

            <div class="tags">
              <ion-chip>
                <ion-icon :icon="pricetag" />
                <ion-label>Shopify ID</ion-label>
              </ion-chip>
              <ion-chip>
                <ion-icon :icon="pricetag" />
                <ion-label>Customer Loyalty Status</ion-label>
              </ion-chip>
            </div>

            <div class="metadata">
              <ion-note>Ordered on 7 Jan 2021</ion-note>
              <ion-badge>Approved</ion-badge>
            </div>
          </section>

          <section class="section-grid">
            <ion-card>
              <ion-item>
                <ion-thumbnail slot="start">
                  <Image />
                </ion-thumbnail>
                <ion-label>
                  <p>Brand</p>
                  Virtual Name
                  <p>{{ $t("Color") }} : color</p>
                  <p>{{ $t("Size") }}: size</p>
                </ion-label>
                <ion-badge color="primary" slot="end">Approved</ion-badge>
              </ion-item>
              <ion-item>
                <ion-label> {{ $t("Promise date") }} </ion-label>
                <p slot="end">14 Jan 2021</p>
              </ion-item>
              <ion-item>
                <ion-label> {{ $t("PO arrival date") }} </ion-label>
                <p slot="end">14 Jan 2021</p>
              </ion-item>
              <ion-item>
                <ion-label> {{ $t("Last brokered") }} </ion-label>
                <p slot="end">California Warehouse</p>
              </ion-item>
            </ion-card>
            <ion-card>
              <ion-item>
                <ion-thumbnail slot="start">
                  <Image />
                </ion-thumbnail>
                <ion-label>
                  <p>Brand</p>
                  Virtual Name
                  <p>{{ $t("Color") }} : color</p>
                  <p>{{ $t("Size") }}: size</p>
                </ion-label>
                <ion-badge color="primary" slot="end">Approved</ion-badge>
              </ion-item>
              <ion-item>
                <ion-label> {{ $t("Promise date") }} </ion-label>
                <p slot="end">14 Jan 2021</p>
              </ion-item>
              <ion-item>
                <ion-label> {{ $t("PO arrival date") }} </ion-label>
                <p slot="end">14 Jan 2021</p>
              </ion-item>
              <ion-item>
                <ion-label> {{ $t("Last brokered") }} </ion-label>
                <p slot="end">California Warehouse</p>
              </ion-item>
            </ion-card>
            <ion-card>
              <ion-item>
                <ion-thumbnail slot="start">
                  <Image />
                </ion-thumbnail>
                <ion-label>
                  <p>Brand</p>
                  Virtual Name
                  <p>{{ $t("Color") }} : color</p>
                  <p>{{ $t("Size") }}: size</p>
                </ion-label>
                <ion-badge color="primary" slot="end">Approved</ion-badge>
              </ion-item>
              <ion-item>
                <ion-label> {{ $t("Promise date") }} </ion-label>
                <p slot="end">14 Jan 2021</p>
              </ion-item>
              <ion-item>
                <ion-label> {{ $t("PO arrival date") }} </ion-label>
                <p slot="end">14 Jan 2021</p>
              </ion-item>
              <ion-item>
                <ion-label> {{ $t("Last brokered") }} </ion-label>
                <p slot="end">California Warehouse</p>
              </ion-item>
            </ion-card>
            <ion-card>
              <ion-item>
                <ion-thumbnail slot="start">
                  <Image />
                </ion-thumbnail>
                <ion-label>
                  <p>Brand</p>
                  Virtual Name
                  <p>{{ $t("Color") }} : color</p>
                  <p>{{ $t("Size") }}: size</p>
                </ion-label>
                <ion-badge color="primary" slot="end">Approved</ion-badge>
              </ion-item>
              <ion-item>
                <ion-label> {{ $t("Promise date") }} </ion-label>
                <p slot="end">14 Jan 2021</p>
              </ion-item>
              <ion-item>
                <ion-label> {{ $t("PO arrival date") }} </ion-label>
                <p slot="end">14 Jan 2021</p>
              </ion-item>
              <ion-item>
                <ion-label> {{ $t("Last brokered") }} </ion-label>
                <p slot="end">California Warehouse</p>
              </ion-item>
            </ion-card>
          </section>

          <hr />
        </main>
      </div>
    </ion-content>
  </ion-page>
</template>

<script>
import Image from "../components/Image.vue";
import {
  IonBackButton,
  IonBadge,
  IonButton,
  IonCard,
  IonCardContent,
  IonCheckbox,
  IonChip,
  IonContent,
  IonHeader,
  IonIcon,
  IonItem,
  IonLabel,
  IonList,
  IonListHeader,
  IonNote,
  IonPage,
  IonSearchbar,
  IonSelect,
  IonThumbnail,
  IonTitle,
  IonToolbar,
  IonSelectOption,
} from "@ionic/vue";
import { pricetag, ribbon, downloadOutline, syncOutline, filterOutline } from "ionicons/icons";
export default {
  name: "Order",
  components: {
    Image,
    IonSelectOption,
    IonBackButton,
    IonBadge,
    IonButton,
    IonCard,
    IonCardContent,
    IonCheckbox,
    IonChip,
    IonContent,
    IonHeader,
    IonIcon,
    IonItem,
    IonLabel,
    IonList,
    IonListHeader,
    IonNote,
    IonPage,
    IonSearchbar,
    IonSelect,
    IonThumbnail,
    IonTitle,
    IonToolbar,
  },
  setup() {
    return {
      pricetag,
      ribbon,
      downloadOutline,
      syncOutline,
      filterOutline
    };
  },
};
</script>

<style scoped>
.metadata {
  text-align: end;
}

.metadata > ion-note {
  display: block;
}

hr {
  border-width: 1px;
  color: var(--ion-color-medium);
}
</style>

