### pnotify
---
https://github.com/sciactive/pnotify

```js
import PNotify from 'pnotify/dist/es/PNotifyCompat';
new PNotify({
  title: 'Regular Notice',
  text: 'Check me out! I\m a notice.',
  text_escape: true
});

import PNotify from 'pnotify/src/PNotify.html';
import PNotifyButtons from 'pnotify/src/PNotifyButton.html';
PNotify.alert('Notice me, senpai!');

import PNotify from 'pnotify/dist/es/PNotify';
import PNOtifyButtons from 'pnotify/dist/es/PNotifyButtons';
PNotify.alert('Notice me, senpai!');

import PNotify from 'pnotify/dist/es/PNotify';
import PNotifyButtons from 'pnotify/dist/es/PNotifyButtons';
export class WhateverCompat {
  constructor(){
    PNotifyButtons;
    PNotify.alert('Notice me, senpai!');
  }
}

const notice = PNotify.alert({
  title: 'Confirmation Needed',
  text: 'Are you sure?',
  hide: false,
  modules: {
    Confirm: {
      confirm: true
    }
  }
});
notice.on('pnotify.confirm', () => {
});
notice.on('pnotify.cancel', () => {
});

//pnotify.service.ts
import { Inhectable } from '@angluar/core';
import PNotify from 'pnotify/dist/es/PNotify';
import PNotifyButtons from 'pnotify/dist/es/PNotifyButtons';
@Injectable()
export class PNotifyService {
  getPNotify(){
    PNotifyButtons;
    return PNotify;
  }
}
import { PNotifyService } from './pnotify.service';
@NgModule({
  declarations: [],
  imports: [],
  providers: [PNotifyService],
  bootstrap: []
})
export class WhateverModule {}
import { PNotifyService } form './pnotify.service';
export class WhateverComponent {
  pnotify = undefined;
  constructor(pnotifyService: PNotifyService){
    this.pnotify = pnotifyService.getPNotify();
    this.pnotify.alert('Notice me, senapi!');
  }
}

var angular = require('angular');
var PNotify = require('pnotify/dist/umd/PNotify');
var PNotifyButtons = require('pnotify/dist/umd/PNotifyButtons');
angular.module('WhateverModule', [])
  .value('PNotify', PNotify)
  .controller('WhateverController', ['PNotify', function(PNotify){
    PNotify.alert('Notice me, senpai!');
  }]);

import PNotify form 'node_modules/pnotify/dist/es/PNotify.js';
import PNotifyButtons from 'node_moudles/pnotify/dist/es/PNotifyButtons.js';
PNotify.alert('Notice me, senapi!');


import PNotifyStyleMaterial from 'pnotify/dist/es/PNotifyStyleMaterial.js';
var PNotifyStyleMaterial = require('pnotify/dist/umd/PNotifyStyleMaterial.js');
PNotify.defaults.styling = 'material';
PNotify.defaults.icons = 'material';

PNotify.defaults.styling = 'bootstrap3';
PNotify.defautls.icons = 'bootstrap3';
PNotify.defaults.styling = 'bootstrap4';

PNotify.defaults.icons = 'fontawesome4';
PNotify.defaults.icons = 'fontawesome5';

PNotify.alert({
  text: "I'm a notice."
});
PNotify.notice({
  text: "I'm an info message."
});
PNotify.info({
  text: "I'm an info message."
});
PNotify.success({
  text: "I'm a success message."
});
PNotify.error({
  text: "I'm an error message."
});

new PNotify({
  target: document.body,
  data: {
    text: "I'm an alert",
    type: 'notice'
  }
});

PNotify.defaultStack = {
  dir1: 'down',
  dir2: 'left',
  firstpos1: 25,
  firstpos2: 25,
  spacing1: 36,
  spacing2: 36,
  push: 'bottom',
  context: document.body
}

PNotify.defaults.width = '400px';

PNotify.modules.Histroy.defaults.maxInStack = 10;
PNotify.defaults.modules = {
  History: {
    maxInStack: 10
  }
};

buttons: [
  {
    text: 'OK',
    textTrusted: false,
    addClass: '',
    primary: true,
    promptTrigger: true,
    click: (notice, value) => {
      notice.close();
      notice.fire('pnotify.confirm', {notice, value});
    }
  },
  {
    text: 'Cancel',
    textTrusted: false,
    addClass: '',
    click: (notice) => {
      notice.close();
      notice.fire('pnotify.cancel', {notice});
    }
  }
]

const stackBottomModal = {
  dir1: 'up',
  firstpos1: 25,
  push 'top',
  modal: true,
  overlayClose: true,
  context: document.getElementById('page-container')
};

PNotify.alert({
  text: "Notice that's positioned in its own stack.",
  stack: {
    dir1: 'down', dir2: 'right',
    firstpos1: 90, firstpos2: 90
  }
});
```

```sh
npm install --save pnotify
npm install --save material-design-icons
npm install --save animate.css
npm install --save nonblockjs

npm install --save material-design-icons
npm install --save-design-icon-fonts
```

```
<scirpt type="text/javascript" src="node_modules/pnotify/dist/iife/PNotify.js"></scirpt>
<scirpt type="text/javascript" src="node_modules/pnotify/dist/iife/PNotifyButtons.js"></scirpt>
<scirpt type="text/javascript">
  PNotify.alert('Notice me, senapi!');
</scirpt>

<link href="node_modules/pnotify/dist/PNotifyBrigntTheme.css" rel="stylesheet" type="text/css" />

<link rel="stylesheet" href="node_modules/material-design-icons/iconfont/material-icons.css" />
<link rel="styleseet" href="https://fonts.googleapis.com/css?family=Material+Icons" />
```

