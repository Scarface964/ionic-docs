---
title: "ion-radio-group"
hide_table_of_contents: true
---
import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';
import TOCInline from '@theme/TOCInline';

import Props from '@site/static/auto-generated/radio-group/props.md';
import Events from '@site/static/auto-generated/radio-group/events.md';
import Methods from '@site/static/auto-generated/radio-group/methods.md';
import Parts from '@site/static/auto-generated/radio-group/parts.md';
import CustomProps from '@site/static/auto-generated/radio-group/custom-props.md';
import Slots from '@site/static/auto-generated/radio-group/slots.md';

<head>
  <title>ion-radio-group | Radio Button Group Usage for Ionic Apps</title>
  <meta name="description" content="A radio group is a group of radio buttons. Radio groups allow a user to select at most one radio button from a set. Learn more about ion-radio-group usage." />
</head>

import EncapsulationPill from '@components/page/api/EncapsulationPill';

<h2 className="table-of-contents__title">Contents</h2>

<TOCInline
  toc={toc}
  maxHeadingLevel={2}
/>



A radio group is a group of [radio buttons](radio.md). It allows
a user to select at most one radio button from a set. Checking one radio
button that belongs to a radio group unchecks any previous checked
radio button within the same group.

## Interfaces

### RadioGroupChangeEventDetail

```typescript
interface RadioGroupChangeEventDetail<T = any> {
  value: T;
}
```

### RadioGroupCustomEvent

While not required, this interface can be used in place of the `CustomEvent` interface for stronger typing with Ionic events emitted from this component.

```typescript
interface RadioGroupCustomEvent<T = any> extends CustomEvent {
  detail: RadioGroupChangeEventDetail<T>;
  target: HTMLIonRadioGroupElement;
}
```



## Usage

<Tabs groupId="framework" defaultValue="angular" values={[{ value: 'angular', label: 'Angular' }, { value: 'javascript', label: 'Javascript' }, { value: 'react', label: 'React' }, { value: 'stencil', label: 'Stencil' }, { value: 'vue', label: 'Vue' }]}>

<TabItem value="angular">

```html
<ion-list>
  <ion-radio-group>
    <ion-list-header>
      <ion-label>
        Auto Manufacturers
      </ion-label>
    </ion-list-header>

    <ion-item>
      <ion-label>Cord</ion-label>
      <ion-radio value="cord"></ion-radio>
    </ion-item>

    <ion-item>
      <ion-label>Duesenberg</ion-label>
      <ion-radio value="duesenberg"></ion-radio>
    </ion-item>

    <ion-item>
      <ion-label>Hudson</ion-label>
      <ion-radio value="hudson"></ion-radio>
    </ion-item>

    <ion-item>
      <ion-label>Packard</ion-label>
      <ion-radio value="packard"></ion-radio>
    </ion-item>

    <ion-item>
      <ion-label>Studebaker</ion-label>
      <ion-radio value="studebaker"></ion-radio>
    </ion-item>
  </ion-radio-group>
</ion-list>
```


</TabItem>


<TabItem value="javascript">

```html
<ion-list>
  <ion-radio-group>
    <ion-list-header>
      <ion-label>
        Auto Manufacturers
      </ion-label>
    </ion-list-header>

    <ion-item>
      <ion-label>Cord</ion-label>
      <ion-radio value="cord"></ion-radio>
    </ion-item>

    <ion-item>
      <ion-label>Duesenberg</ion-label>
      <ion-radio value="duesenberg"></ion-radio>
    </ion-item>

    <ion-item>
      <ion-label>Hudson</ion-label>
      <ion-radio value="hudson"></ion-radio>
    </ion-item>

    <ion-item>
      <ion-label>Packard</ion-label>
      <ion-radio value="packard"></ion-radio>
    </ion-item>

    <ion-item>
      <ion-label>Studebaker</ion-label>
      <ion-radio value="studebaker"></ion-radio>
    </ion-item>
  </ion-radio-group>
</ion-list>
```


</TabItem>


<TabItem value="react">

```tsx
import React from 'react';
import { IonList, IonRadioGroup, IonListHeader, IonLabel, IonRadio, IonItem, IonContent } from '@ionic/react';

export const RadioGroupExample: React.FC = () => (
  <IonContent>
    <IonList>
      <IonRadioGroup>
        <IonListHeader>
          <IonLabel>
            Auto Manufacturers
          </IonLabel>
        </IonListHeader>

        <IonItem>
          <IonLabel>Cord</IonLabel>
          <IonRadio value="cord" />
        </IonItem>

        <IonItem>
          <IonLabel>Duesenberg</IonLabel>
          <IonRadio value="duesenberg" />
        </IonItem>

        <IonItem>
          <IonLabel>Hudson</IonLabel>
          <IonRadio value="hudson" />
        </IonItem>

        <IonItem>
          <IonLabel>Packard</IonLabel>
          <IonRadio value="packard" />
        </IonItem>

        <IonItem>
          <IonLabel>Studebaker</IonLabel>
          <IonRadio value="studebaker" />
        </IonItem>
      </IonRadioGroup>
    </IonList>
  </IonContent>
);
```

</TabItem>


<TabItem value="stencil">

```tsx
import { Component, h } from '@stencil/core';

@Component({
  tag: 'radio-group-example',
  styleUrl: 'radio-group-example.css'
})
export class RadioGroupExample {
  render() {
    return [
      <ion-list>
        <ion-radio-group>
          <ion-list-header>
            <ion-label>
              Auto Manufacturers
            </ion-label>
          </ion-list-header>

          <ion-item>
            <ion-label>Cord</ion-label>
            <ion-radio value="cord"></ion-radio>
          </ion-item>

          <ion-item>
            <ion-label>Duesenberg</ion-label>
            <ion-radio value="duesenberg"></ion-radio>
          </ion-item>

          <ion-item>
            <ion-label>Hudson</ion-label>
            <ion-radio value="hudson"></ion-radio>
          </ion-item>

          <ion-item>
            <ion-label>Packard</ion-label>
            <ion-radio value="packard"></ion-radio>
          </ion-item>

          <ion-item>
            <ion-label>Studebaker</ion-label>
            <ion-radio value="studebaker"></ion-radio>
          </ion-item>
        </ion-radio-group>
      </ion-list>
    ];
  }
}
```


</TabItem>


<TabItem value="vue">

```html
<template>
  <ion-list>
    <ion-radio-group>
      <ion-list-header>
        <ion-label>
          Auto Manufacturers
        </ion-label>
      </ion-list-header>

      <ion-item>
        <ion-label>Cord</ion-label>
        <ion-radio value="cord"></ion-radio>
      </ion-item>

      <ion-item>
        <ion-label>Duesenberg</ion-label>
        <ion-radio value="duesenberg"></ion-radio>
      </ion-item>

      <ion-item>
        <ion-label>Hudson</ion-label>
        <ion-radio value="hudson"></ion-radio>
      </ion-item>

      <ion-item>
        <ion-label>Packard</ion-label>
        <ion-radio value="packard"></ion-radio>
      </ion-item>

      <ion-item>
        <ion-label>Studebaker</ion-label>
        <ion-radio value="studebaker"></ion-radio>
      </ion-item>
    </ion-radio-group>
  </ion-list>
</template>

<script>
import { 
  IonItem, 
  IonLabel, 
  IonList, 
  IonListHeader, 
  IonRadio, 
  IonRadioGroup
} from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  components: {
    IonItem, 
    IonLabel, 
    IonList, 
    IonListHeader, 
    IonRadio, 
    IonRadioGroup
  }
});
</script>
```


</TabItem>

</Tabs>

## Properties
<Props />

## Events
<Events />

## Methods
<Methods />

## CSS Shadow Parts
<Parts />

## CSS Custom Properties
<CustomProps />

## Slots
<Slots />