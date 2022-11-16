<template>
   <v-navigation-drawer app color="white" right width="290">
        <v-list subheader two-line class="mt-1">
            <v-list-item>
                <v-list-item-avatar rounded>
                    <v-img src="https://cdn.vuetifyjs.com/images/lists/2.jpg"></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                    <v-list-item-subtitle>I'm a Cashiter</v-list-item-subtitle>
                    <v-list-item-title>Jelly Grande</v-list-item-title>
                </v-list-item-content>
                <v-list-item-action>
                    <v-badge bordered overlap color="red" dot>
                        <v-icon>far fa-bell</v-icon>
                    </v-badge>
                </v-list-item-action>
            </v-list-item>
        </v-list>
        <strong class="ml-3">Bills</strong>
        <v-list subheader two-line class="mt-1">
            <v-list-item>
                <v-list-item-avatar rounded color="grey lighten-4">
                    <v-img src="https://globalassets.starbucks.com/assets/410cd92738514641bf497d4b6a18c30f.jpg?impolicy=1by1_wide_topcrop_630"></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                    <v-list-item-title class="subtitle-2">Caramel Frappuccino</v-list-item-title>
                    <v-list-item-subtitle>X1
                        <v-btn plain color="#704232" small>Notes
                            <v-icon right>mdi-pencil</v-icon>
                        </v-btn>
                    </v-list-item-subtitle>
                </v-list-item-content>
                <v-list-item-action class="caption">$3.95</v-list-item-action>
            </v-list-item>
        </v-list>
        <v-list subheader two-line class="mt-1">
            <v-list-item>
                <v-list-item-avatar rounded color="grey lighten-4">
                    <v-img src="data:image/jpeg;base64,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"></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                    <v-list-item-title class="subtitle-2">Chocolate Frappucino</v-list-item-title>
                    <v-list-item-subtitle>X1
                        <v-btn plain color="#704232" small>Notes
                            <v-icon right>mdi-pencil</v-icon>
                        </v-btn>
                    </v-list-item-subtitle>
                </v-list-item-content>
                <v-list-item-action class="caption">$9.05</v-list-item-action>
            </v-list-item>
        </v-list>
        <v-list subheader two-line class="mt-1">
            <v-list-item>
                <v-list-item-avatar rounded color="grey lighten-4">
                    <v-img src="https://globalassets.starbucks.com/assets/9c7cbbff6b6e4b2a8a9bd403e83dcdde.jpg?impolicy=1by1_wide_topcrop_630"></v-img>
                </v-list-item-avatar>
                <v-list-item-content>
                    <v-list-item-title class="subtitle-2">Peppermint Macchiato</v-list-item-title>
                    <v-list-item-subtitle>X1
                        <v-btn plain color="#704232" small>Notes
                            <v-icon right>mdi-pencil</v-icon>
                        </v-btn>
                    </v-list-item-subtitle>
                </v-list-item-content>
                <v-list-item-action class="caption">$5.34</v-list-item-action>
            </v-list-item>
        </v-list>
        <v-toolbar color="rgba(0,0,0,0)" flat>
            <strong>Subtotal</strong><v-spacer></v-spacer><strong>$18.34</strong>
        </v-toolbar>
        <v-toolbar color="rgba(0,0,0,0)" flat class="mt-n6">
            <span>Tax(10%)</span><v-spacer></v-spacer><span>$1.831</span>
        </v-toolbar>
        <v-divider class="mx-4"></v-divider>
        <v-toolbar color="rgba(0,0,0,0)" flat>
            <strong>Total</strong><v-spacer></v-spacer><span>$20.171</span>
        </v-toolbar>
        <strong class="ml-5">Payment Method</strong>
        <v-item-group mandatory class="mt-n1">
            <v-container>
                <v-row justify="center">
                    <v-col cols="12" md="4">
                        <v-item v-slot="{active, toggle}">
                            <v-card color="#F6EFEF" :class="active ? 'borderme' : ''" class="d-flex align0center rounded-lg" dark height="70" @click="toggle" flat>
                                <v-row>
                                    <v-col cols="12" md="12">
                                        <v-list-item three-line class="text-center mt-1">
                                            <v-list-item-content>
                                                <div>
                                                    <v-icon :color="active ? '#704232' : 'black'">fas fa-money-bill-wave</v-icon>
                                                </div>
                                                <v-list-item-subtitle :class="active ? 'brown--text' : 'black--text'" class="mt-n2 caption">
                                                    Catch
                                                </v-list-item-subtitle>
                                            </v-list-item-content>
                                        </v-list-item>
                                    </v-col>
                                </v-row>
                            </v-card>
                        </v-item>
                    </v-col>
                    <v-col cols="12" md="4">
                        <v-item v-slot="{active, toggle}">
                            <v-card color="#F6EFEF" :class="active ? 'borderme' : ''" class="d-flex align0center rounded-lg" dark height="70" @click="toggle" flat>
                                <v-row>
                                    <v-col cols="12" md="12">
                                        <v-list-item three-line class="text-center mt-1">
                                            <v-list-item-content>
                                                <div>
                                                    <v-icon :color="active ? '#704232' : 'black'">fas fa-credit-card</v-icon>
                                                </div>
                                                <v-list-item-subtitle :class="active ? 'brown--text' : 'black--text'" class="mt-n2 caption">
                                                    debit Card
                                                </v-list-item-subtitle>
                                            </v-list-item-content>
                                        </v-list-item>
                                    </v-col>
                                </v-row>
                            </v-card>
                        </v-item>
                    </v-col>
                    <v-col cols="12" md="4">
                        <v-item v-slot="{active, toggle}">
                            <v-card color="#F6EFEF" :class="active ? 'borderme' : ''" class="d-flex align0center rounded-lg" dark height="70" @click="toggle" flat>
                                <v-row>
                                    <v-col cols="12" md="12">
                                        <v-list-item three-line class="text-center mt-1">
                                            <v-list-item-content>
                                                <div>
                                                    <v-icon :color="active ? '#704232' : 'black'">fas fa-qrcode</v-icon>
                                                </div>
                                                <v-list-item-subtitle :class="active ? 'brown--text' : 'black--text'" class="mt-n2 caption">
                                                    E-Wallet
                                                </v-list-item-subtitle>
                                            </v-list-item-content>
                                        </v-list-item>
                                    </v-col>
                                </v-row>
                            </v-card>
                        </v-item>
                    </v-col>
                </v-row>
            </v-container>
        </v-item-group>
        <div class="mx-3 mt-2">
            <v-btn color="704232" block dark class="widthoutupercase">Print Bills</v-btn>
        </div>
   </v-navigation-drawer>
</template>

<script>
export default {

}
</script>

<style>
    .v-card.borderme{
        border: 2px solid #704232 !important;
    }
    .col-12{
        padding: 5px !important;
    }
    .v-btn.widthoutupercase{
        text-transform: none !important;
    }
</style>