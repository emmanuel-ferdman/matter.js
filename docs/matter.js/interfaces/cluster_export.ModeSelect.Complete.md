[@project-chip/matter.js](../README.md) / [Modules](../modules.md) / [cluster/export](../modules/cluster_export.md) / [ModeSelect](../modules/cluster_export.ModeSelect.md) / Complete

# Interface: Complete

[cluster/export](../modules/cluster_export.md).[ModeSelect](../modules/cluster_export.ModeSelect.md).Complete

This cluster supports all ModeSelect features. It may support illegal feature combinations.

If you use this cluster you must manually specify which features are active and ensure the set of active
features is legal per the Matter specification.

## Hierarchy

- [`Identity`](../modules/util_export.md#identity)\<typeof [`CompleteInstance`](../modules/cluster_export.ModeSelect.md#completeinstance)\>

  ↳ **`Complete`**

## Table of contents

### Properties

- [attributes](cluster_export.ModeSelect.Complete.md#attributes)
- [base](cluster_export.ModeSelect.Complete.md#base)
- [commands](cluster_export.ModeSelect.Complete.md#commands)
- [events](cluster_export.ModeSelect.Complete.md#events)
- [extensions](cluster_export.ModeSelect.Complete.md#extensions)
- [features](cluster_export.ModeSelect.Complete.md#features)
- [id](cluster_export.ModeSelect.Complete.md#id)
- [name](cluster_export.ModeSelect.Complete.md#name)
- [revision](cluster_export.ModeSelect.Complete.md#revision)
- [supportedFeatures](cluster_export.ModeSelect.Complete.md#supportedfeatures)
- [unknown](cluster_export.ModeSelect.Complete.md#unknown)

### Methods

- [alter](cluster_export.ModeSelect.Complete.md#alter)
- [enable](cluster_export.ModeSelect.Complete.md#enable)
- [set](cluster_export.ModeSelect.Complete.md#set)
- [with](cluster_export.ModeSelect.Complete.md#with)

## Properties

### attributes

• **attributes**: [`Merge`](../modules/util_export.md#merge)\<\{ `acceptedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `attributeList`: [`Attribute`](cluster_export.Attribute.md)\<[`AttributeId`](../modules/datatype_export.md#attributeid)[], `never`\> ; `clusterRevision`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `never`\> ; `currentMode`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `any`\> ; `description`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<`string`, `any`\> ; `eventList`: [`Attribute`](cluster_export.Attribute.md)\<[`EventId`](../modules/datatype_export.md#eventid)[], `never`\> ; `featureMap`: [`Attribute`](cluster_export.Attribute.md)\<[`TypeFromPartialBitSchema`](../modules/schema_export.md#typefrompartialbitschema)\<\{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  }\>, `never`\> ; `generatedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `onMode`: [`WritableAttribute`](cluster_export.WritableAttribute.md)\<``null`` \| `number`, `any`\> & \{ `isConditional`: ``true`` = true; `mandatoryIf`: [] \| [\{ `onOff`: `boolean` = true }] ; `optional`: ``true`` = true; `optionalIf`: [] \| [`ConditionalFeatureList`](../modules/cluster_export.md#conditionalfeaturelist)\<[`BitSchema`](../modules/schema_export.md#bitschema)\>  } ; `standardNamespace`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<``null`` \| `number`, `any`\> ; `startUpMode`: [`OptionalWritableAttribute`](cluster_export.OptionalWritableAttribute.md)\<``null`` \| `number`, `any`\> ; `supportedModes`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `label`: [`FieldType`](tlv_export.FieldType.md)\<`string`\> ; `mode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\> ; `semanticTags`: [`FieldType`](tlv_export.FieldType.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `mfgCode`: [`FieldType`](tlv_export.FieldType.md)\<...\> ; `value`: [`FieldType`](tlv_export.FieldType.md)\<...\>  }\>[]\>  }\>[], `any`\>  }, [`GlobalAttributes`](../modules/cluster_export.md#globalattributes)\<\{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  }\>\>

#### Inherited from

Identity.attributes

#### Defined in

[packages/matter.js/src/cluster/ClusterType.ts:86](https://github.com/project-chip/matter.js/blob/3adaded6/packages/matter.js/src/cluster/ClusterType.ts#L86)

___

### base

• **base**: `undefined`

#### Inherited from

Identity.base

#### Defined in

[packages/matter.js/src/cluster/ClusterType.ts:92](https://github.com/project-chip/matter.js/blob/3adaded6/packages/matter.js/src/cluster/ClusterType.ts#L92)

___

### commands

• **commands**: `Object`

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `changeToMode` | [`Command`](cluster_export.Command.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `newMode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\>  }\>, `void`, `any`\> | On receipt of this command, if the NewMode field indicates a valid mode transition within the supported list, the server shall set the CurrentMode attribute to the NewMode value, otherwise, the server shall respond with an INVALID_COMMAND status response. **`See`** [MatterApplicationClusterSpecificationV1_1](spec_export.MatterApplicationClusterSpecificationV1_1.md) § 1.8.6.1 |

#### Inherited from

Identity.commands

#### Defined in

[packages/matter.js/src/cluster/ClusterType.ts:89](https://github.com/project-chip/matter.js/blob/3adaded6/packages/matter.js/src/cluster/ClusterType.ts#L89)

___

### events

• **events**: `Object`

#### Inherited from

Identity.events

#### Defined in

[packages/matter.js/src/cluster/ClusterType.ts:90](https://github.com/project-chip/matter.js/blob/3adaded6/packages/matter.js/src/cluster/ClusterType.ts#L90)

___

### extensions

• **extensions**: `undefined`

#### Inherited from

Identity.extensions

#### Defined in

[packages/matter.js/src/cluster/ClusterType.ts:93](https://github.com/project-chip/matter.js/blob/3adaded6/packages/matter.js/src/cluster/ClusterType.ts#L93)

___

### features

• **features**: `Object`

#### Type declaration

| Name | Type | Description |
| :------ | :------ | :------ |
| `onOff` | [`BitFlag`](../modules/schema_export.md#bitflag) | OnOff Dependency with the On/Off cluster |

#### Inherited from

Identity.features

#### Defined in

[packages/matter.js/src/cluster/ClusterType.ts:84](https://github.com/project-chip/matter.js/blob/3adaded6/packages/matter.js/src/cluster/ClusterType.ts#L84)

___

### id

• **id**: [`Branded`](../modules/util_export.md#branded)\<[`Branded`](../modules/util_export.md#branded)\<``80``, ``"ClusterId"``\>, ``"ClusterId"``\>

#### Inherited from

Identity.id

#### Defined in

[packages/matter.js/src/cluster/ClusterType.ts:81](https://github.com/project-chip/matter.js/blob/3adaded6/packages/matter.js/src/cluster/ClusterType.ts#L81)

___

### name

• **name**: ``"ModeSelect"``

#### Inherited from

Identity.name

#### Defined in

[packages/matter.js/src/cluster/ClusterType.ts:82](https://github.com/project-chip/matter.js/blob/3adaded6/packages/matter.js/src/cluster/ClusterType.ts#L82)

___

### revision

• **revision**: ``1``

#### Inherited from

Identity.revision

#### Defined in

[packages/matter.js/src/cluster/ClusterType.ts:83](https://github.com/project-chip/matter.js/blob/3adaded6/packages/matter.js/src/cluster/ClusterType.ts#L83)

___

### supportedFeatures

• **supportedFeatures**: `Object`

#### Inherited from

Identity.supportedFeatures

#### Defined in

[packages/matter.js/src/cluster/ClusterType.ts:85](https://github.com/project-chip/matter.js/blob/3adaded6/packages/matter.js/src/cluster/ClusterType.ts#L85)

___

### unknown

• **unknown**: ``false``

#### Inherited from

Identity.unknown

#### Defined in

[packages/matter.js/src/cluster/ClusterType.ts:91](https://github.com/project-chip/matter.js/blob/3adaded6/packages/matter.js/src/cluster/ClusterType.ts#L91)

## Methods

### alter

▸ **alter**\<`AlterationsT`\>(`alterations`): [`WithAlterations`](../modules/cluster_export.ElementModifier.md#withalterations)\<[`Of`](cluster_export.ClusterType.Of.md)\<\{ `attributes`: \{ `acceptedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `attributeList`: [`Attribute`](cluster_export.Attribute.md)\<[`AttributeId`](../modules/datatype_export.md#attributeid)[], `never`\> ; `clusterRevision`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `never`\> ; `currentMode`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `any`\> ; `description`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<`string`, `any`\> ; `eventList`: [`Attribute`](cluster_export.Attribute.md)\<[`EventId`](../modules/datatype_export.md#eventid)[], `never`\> ; `featureMap`: [`Attribute`](cluster_export.Attribute.md)\<[`TypeFromPartialBitSchema`](../modules/schema_export.md#typefrompartialbitschema)\<\{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  }\>, `never`\> ; `generatedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `onMode`: [`WritableAttribute`](cluster_export.WritableAttribute.md)\<``null`` \| `number`, `any`\> & \{ `isConditional`: ``true`` = true; `mandatoryIf`: [] \| [\{ `onOff`: `boolean` = true }] ; `optional`: ``true`` = true; `optionalIf`: [] \| [`ConditionalFeatureList`](../modules/cluster_export.md#conditionalfeaturelist)\<[`BitSchema`](../modules/schema_export.md#bitschema)\>  } ; `standardNamespace`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<``null`` \| `number`, `any`\> ; `startUpMode`: [`OptionalWritableAttribute`](cluster_export.OptionalWritableAttribute.md)\<``null`` \| `number`, `any`\> ; `supportedModes`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `label`: [`FieldType`](tlv_export.FieldType.md)\<`string`\> ; `mode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\> ; `semanticTags`: [`FieldType`](tlv_export.FieldType.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<...\>[]\>  }\>[], `any`\>  } ; `commands`: \{ `changeToMode`: [`Command`](cluster_export.Command.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `newMode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\>  }\>, `void`, `any`\>  } = Cluster.commands; `features`: \{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  } = Cluster.features; `id`: [`Branded`](../modules/util_export.md#branded)\<``80``, ``"ClusterId"``\> = Cluster.id; `name`: ``"ModeSelect"`` = Cluster.name; `revision`: ``1`` = Cluster.revision }\>, `AlterationsT`\>

Modify elements using [ElementModifier.alter](../classes/cluster_export.ElementModifier-1.md#alter).

#### Type parameters

| Name | Type |
| :------ | :------ |
| `AlterationsT` | extends [`Alterations`](../modules/cluster_export.ElementModifier.md#alterations)\<[`Of`](cluster_export.ClusterType.Of.md)\<\{ `attributes`: \{ `acceptedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `attributeList`: [`Attribute`](cluster_export.Attribute.md)\<[`AttributeId`](../modules/datatype_export.md#attributeid)[], `never`\> ; `clusterRevision`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `never`\> ; `currentMode`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `any`\> ; `description`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<`string`, `any`\> ; `eventList`: [`Attribute`](cluster_export.Attribute.md)\<[`EventId`](../modules/datatype_export.md#eventid)[], `never`\> ; `featureMap`: [`Attribute`](cluster_export.Attribute.md)\<[`TypeFromPartialBitSchema`](../modules/schema_export.md#typefrompartialbitschema)\<\{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  }\>, `never`\> ; `generatedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `onMode`: [`WritableAttribute`](cluster_export.WritableAttribute.md)\<``null`` \| `number`, `any`\> & \{ `isConditional`: ``true`` = true; `mandatoryIf`: [] \| [\{ `onOff`: `boolean` = true }] ; `optional`: ``true`` = true; `optionalIf`: [] \| [`ConditionalFeatureList`](../modules/cluster_export.md#conditionalfeaturelist)\<[`BitSchema`](../modules/schema_export.md#bitschema)\>  } ; `standardNamespace`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<``null`` \| `number`, `any`\> ; `startUpMode`: [`OptionalWritableAttribute`](cluster_export.OptionalWritableAttribute.md)\<``null`` \| `number`, `any`\> ; `supportedModes`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `label`: [`FieldType`](tlv_export.FieldType.md)\<`string`\> ; `mode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\> ; `semanticTags`: [`FieldType`](tlv_export.FieldType.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<...\>[]\>  }\>[], `any`\>  } ; `commands`: \{ `changeToMode`: [`Command`](cluster_export.Command.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `newMode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\>  }\>, `void`, `any`\>  } = Cluster.commands; `features`: \{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  } = Cluster.features; `id`: [`Branded`](../modules/util_export.md#branded)\<``80``, ``"ClusterId"``\> = Cluster.id; `name`: ``"ModeSelect"`` = Cluster.name; `revision`: ``1`` = Cluster.revision }\>\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `alterations` | `AlterationsT` |

#### Returns

[`WithAlterations`](../modules/cluster_export.ElementModifier.md#withalterations)\<[`Of`](cluster_export.ClusterType.Of.md)\<\{ `attributes`: \{ `acceptedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `attributeList`: [`Attribute`](cluster_export.Attribute.md)\<[`AttributeId`](../modules/datatype_export.md#attributeid)[], `never`\> ; `clusterRevision`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `never`\> ; `currentMode`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `any`\> ; `description`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<`string`, `any`\> ; `eventList`: [`Attribute`](cluster_export.Attribute.md)\<[`EventId`](../modules/datatype_export.md#eventid)[], `never`\> ; `featureMap`: [`Attribute`](cluster_export.Attribute.md)\<[`TypeFromPartialBitSchema`](../modules/schema_export.md#typefrompartialbitschema)\<\{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  }\>, `never`\> ; `generatedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `onMode`: [`WritableAttribute`](cluster_export.WritableAttribute.md)\<``null`` \| `number`, `any`\> & \{ `isConditional`: ``true`` = true; `mandatoryIf`: [] \| [\{ `onOff`: `boolean` = true }] ; `optional`: ``true`` = true; `optionalIf`: [] \| [`ConditionalFeatureList`](../modules/cluster_export.md#conditionalfeaturelist)\<[`BitSchema`](../modules/schema_export.md#bitschema)\>  } ; `standardNamespace`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<``null`` \| `number`, `any`\> ; `startUpMode`: [`OptionalWritableAttribute`](cluster_export.OptionalWritableAttribute.md)\<``null`` \| `number`, `any`\> ; `supportedModes`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `label`: [`FieldType`](tlv_export.FieldType.md)\<`string`\> ; `mode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\> ; `semanticTags`: [`FieldType`](tlv_export.FieldType.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<...\>[]\>  }\>[], `any`\>  } ; `commands`: \{ `changeToMode`: [`Command`](cluster_export.Command.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `newMode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\>  }\>, `void`, `any`\>  } = Cluster.commands; `features`: \{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  } = Cluster.features; `id`: [`Branded`](../modules/util_export.md#branded)\<``80``, ``"ClusterId"``\> = Cluster.id; `name`: ``"ModeSelect"`` = Cluster.name; `revision`: ``1`` = Cluster.revision }\>, `AlterationsT`\>

#### Inherited from

Identity.alter

#### Defined in

[packages/matter.js/src/cluster/mutation/MutableCluster.ts:74](https://github.com/project-chip/matter.js/blob/3adaded6/packages/matter.js/src/cluster/mutation/MutableCluster.ts#L74)

___

### enable

▸ **enable**\<`FlagsT`\>(`flags`): [`WithFlags`](../modules/cluster_export.ElementModifier.md#withflags)\<[`Of`](cluster_export.ClusterType.Of.md)\<\{ `attributes`: \{ `acceptedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `attributeList`: [`Attribute`](cluster_export.Attribute.md)\<[`AttributeId`](../modules/datatype_export.md#attributeid)[], `never`\> ; `clusterRevision`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `never`\> ; `currentMode`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `any`\> ; `description`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<`string`, `any`\> ; `eventList`: [`Attribute`](cluster_export.Attribute.md)\<[`EventId`](../modules/datatype_export.md#eventid)[], `never`\> ; `featureMap`: [`Attribute`](cluster_export.Attribute.md)\<[`TypeFromPartialBitSchema`](../modules/schema_export.md#typefrompartialbitschema)\<\{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  }\>, `never`\> ; `generatedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `onMode`: [`WritableAttribute`](cluster_export.WritableAttribute.md)\<``null`` \| `number`, `any`\> & \{ `isConditional`: ``true`` = true; `mandatoryIf`: [] \| [\{ `onOff`: `boolean` = true }] ; `optional`: ``true`` = true; `optionalIf`: [] \| [`ConditionalFeatureList`](../modules/cluster_export.md#conditionalfeaturelist)\<[`BitSchema`](../modules/schema_export.md#bitschema)\>  } ; `standardNamespace`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<``null`` \| `number`, `any`\> ; `startUpMode`: [`OptionalWritableAttribute`](cluster_export.OptionalWritableAttribute.md)\<``null`` \| `number`, `any`\> ; `supportedModes`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `label`: [`FieldType`](tlv_export.FieldType.md)\<`string`\> ; `mode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\> ; `semanticTags`: [`FieldType`](tlv_export.FieldType.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<...\>[]\>  }\>[], `any`\>  } ; `commands`: \{ `changeToMode`: [`Command`](cluster_export.Command.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `newMode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\>  }\>, `void`, `any`\>  } = Cluster.commands; `features`: \{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  } = Cluster.features; `id`: [`Branded`](../modules/util_export.md#branded)\<``80``, ``"ClusterId"``\> = Cluster.id; `name`: ``"ModeSelect"`` = Cluster.name; `revision`: ``1`` = Cluster.revision }\>, `FlagsT`\>

Modify elements using [ElementModifier.enable](../classes/cluster_export.ElementModifier-1.md#enable).

#### Type parameters

| Name | Type |
| :------ | :------ |
| `FlagsT` | extends [`ElementFlags`](../modules/cluster_export.ElementModifier.md#elementflags)\<[`Of`](cluster_export.ClusterType.Of.md)\<\{ `attributes`: \{ `acceptedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `attributeList`: [`Attribute`](cluster_export.Attribute.md)\<[`AttributeId`](../modules/datatype_export.md#attributeid)[], `never`\> ; `clusterRevision`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `never`\> ; `currentMode`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `any`\> ; `description`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<`string`, `any`\> ; `eventList`: [`Attribute`](cluster_export.Attribute.md)\<[`EventId`](../modules/datatype_export.md#eventid)[], `never`\> ; `featureMap`: [`Attribute`](cluster_export.Attribute.md)\<[`TypeFromPartialBitSchema`](../modules/schema_export.md#typefrompartialbitschema)\<\{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  }\>, `never`\> ; `generatedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `onMode`: [`WritableAttribute`](cluster_export.WritableAttribute.md)\<``null`` \| `number`, `any`\> & \{ `isConditional`: ``true`` = true; `mandatoryIf`: [] \| [\{ `onOff`: `boolean` = true }] ; `optional`: ``true`` = true; `optionalIf`: [] \| [`ConditionalFeatureList`](../modules/cluster_export.md#conditionalfeaturelist)\<[`BitSchema`](../modules/schema_export.md#bitschema)\>  } ; `standardNamespace`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<``null`` \| `number`, `any`\> ; `startUpMode`: [`OptionalWritableAttribute`](cluster_export.OptionalWritableAttribute.md)\<``null`` \| `number`, `any`\> ; `supportedModes`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `label`: [`FieldType`](tlv_export.FieldType.md)\<`string`\> ; `mode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\> ; `semanticTags`: [`FieldType`](tlv_export.FieldType.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<...\>[]\>  }\>[], `any`\>  } ; `commands`: \{ `changeToMode`: [`Command`](cluster_export.Command.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `newMode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\>  }\>, `void`, `any`\>  } = Cluster.commands; `features`: \{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  } = Cluster.features; `id`: [`Branded`](../modules/util_export.md#branded)\<``80``, ``"ClusterId"``\> = Cluster.id; `name`: ``"ModeSelect"`` = Cluster.name; `revision`: ``1`` = Cluster.revision }\>\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `flags` | `FlagsT` |

#### Returns

[`WithFlags`](../modules/cluster_export.ElementModifier.md#withflags)\<[`Of`](cluster_export.ClusterType.Of.md)\<\{ `attributes`: \{ `acceptedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `attributeList`: [`Attribute`](cluster_export.Attribute.md)\<[`AttributeId`](../modules/datatype_export.md#attributeid)[], `never`\> ; `clusterRevision`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `never`\> ; `currentMode`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `any`\> ; `description`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<`string`, `any`\> ; `eventList`: [`Attribute`](cluster_export.Attribute.md)\<[`EventId`](../modules/datatype_export.md#eventid)[], `never`\> ; `featureMap`: [`Attribute`](cluster_export.Attribute.md)\<[`TypeFromPartialBitSchema`](../modules/schema_export.md#typefrompartialbitschema)\<\{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  }\>, `never`\> ; `generatedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `onMode`: [`WritableAttribute`](cluster_export.WritableAttribute.md)\<``null`` \| `number`, `any`\> & \{ `isConditional`: ``true`` = true; `mandatoryIf`: [] \| [\{ `onOff`: `boolean` = true }] ; `optional`: ``true`` = true; `optionalIf`: [] \| [`ConditionalFeatureList`](../modules/cluster_export.md#conditionalfeaturelist)\<[`BitSchema`](../modules/schema_export.md#bitschema)\>  } ; `standardNamespace`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<``null`` \| `number`, `any`\> ; `startUpMode`: [`OptionalWritableAttribute`](cluster_export.OptionalWritableAttribute.md)\<``null`` \| `number`, `any`\> ; `supportedModes`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `label`: [`FieldType`](tlv_export.FieldType.md)\<`string`\> ; `mode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\> ; `semanticTags`: [`FieldType`](tlv_export.FieldType.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<...\>[]\>  }\>[], `any`\>  } ; `commands`: \{ `changeToMode`: [`Command`](cluster_export.Command.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `newMode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\>  }\>, `void`, `any`\>  } = Cluster.commands; `features`: \{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  } = Cluster.features; `id`: [`Branded`](../modules/util_export.md#branded)\<``80``, ``"ClusterId"``\> = Cluster.id; `name`: ``"ModeSelect"`` = Cluster.name; `revision`: ``1`` = Cluster.revision }\>, `FlagsT`\>

#### Inherited from

Identity.enable

#### Defined in

[packages/matter.js/src/cluster/mutation/MutableCluster.ts:88](https://github.com/project-chip/matter.js/blob/3adaded6/packages/matter.js/src/cluster/mutation/MutableCluster.ts#L88)

___

### set

▸ **set**\<`ValuesT`\>(`values`): [`WithValues`](../modules/cluster_export.ElementModifier.md#withvalues)\<[`Of`](cluster_export.ClusterType.Of.md)\<\{ `attributes`: \{ `acceptedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `attributeList`: [`Attribute`](cluster_export.Attribute.md)\<[`AttributeId`](../modules/datatype_export.md#attributeid)[], `never`\> ; `clusterRevision`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `never`\> ; `currentMode`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `any`\> ; `description`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<`string`, `any`\> ; `eventList`: [`Attribute`](cluster_export.Attribute.md)\<[`EventId`](../modules/datatype_export.md#eventid)[], `never`\> ; `featureMap`: [`Attribute`](cluster_export.Attribute.md)\<[`TypeFromPartialBitSchema`](../modules/schema_export.md#typefrompartialbitschema)\<\{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  }\>, `never`\> ; `generatedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `onMode`: [`WritableAttribute`](cluster_export.WritableAttribute.md)\<``null`` \| `number`, `any`\> & \{ `isConditional`: ``true`` = true; `mandatoryIf`: [] \| [\{ `onOff`: `boolean` = true }] ; `optional`: ``true`` = true; `optionalIf`: [] \| [`ConditionalFeatureList`](../modules/cluster_export.md#conditionalfeaturelist)\<[`BitSchema`](../modules/schema_export.md#bitschema)\>  } ; `standardNamespace`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<``null`` \| `number`, `any`\> ; `startUpMode`: [`OptionalWritableAttribute`](cluster_export.OptionalWritableAttribute.md)\<``null`` \| `number`, `any`\> ; `supportedModes`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `label`: [`FieldType`](tlv_export.FieldType.md)\<`string`\> ; `mode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\> ; `semanticTags`: [`FieldType`](tlv_export.FieldType.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<...\>[]\>  }\>[], `any`\>  } ; `commands`: \{ `changeToMode`: [`Command`](cluster_export.Command.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `newMode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\>  }\>, `void`, `any`\>  } = Cluster.commands; `features`: \{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  } = Cluster.features; `id`: [`Branded`](../modules/util_export.md#branded)\<``80``, ``"ClusterId"``\> = Cluster.id; `name`: ``"ModeSelect"`` = Cluster.name; `revision`: ``1`` = Cluster.revision }\>, `ValuesT`\>

Modify elements using [ElementModifier.set](../classes/cluster_export.ElementModifier-1.md#set).

#### Type parameters

| Name | Type |
| :------ | :------ |
| `ValuesT` | extends `Object` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `values` | `ValuesT` |

#### Returns

[`WithValues`](../modules/cluster_export.ElementModifier.md#withvalues)\<[`Of`](cluster_export.ClusterType.Of.md)\<\{ `attributes`: \{ `acceptedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `attributeList`: [`Attribute`](cluster_export.Attribute.md)\<[`AttributeId`](../modules/datatype_export.md#attributeid)[], `never`\> ; `clusterRevision`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `never`\> ; `currentMode`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `any`\> ; `description`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<`string`, `any`\> ; `eventList`: [`Attribute`](cluster_export.Attribute.md)\<[`EventId`](../modules/datatype_export.md#eventid)[], `never`\> ; `featureMap`: [`Attribute`](cluster_export.Attribute.md)\<[`TypeFromPartialBitSchema`](../modules/schema_export.md#typefrompartialbitschema)\<\{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  }\>, `never`\> ; `generatedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `onMode`: [`WritableAttribute`](cluster_export.WritableAttribute.md)\<``null`` \| `number`, `any`\> & \{ `isConditional`: ``true`` = true; `mandatoryIf`: [] \| [\{ `onOff`: `boolean` = true }] ; `optional`: ``true`` = true; `optionalIf`: [] \| [`ConditionalFeatureList`](../modules/cluster_export.md#conditionalfeaturelist)\<[`BitSchema`](../modules/schema_export.md#bitschema)\>  } ; `standardNamespace`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<``null`` \| `number`, `any`\> ; `startUpMode`: [`OptionalWritableAttribute`](cluster_export.OptionalWritableAttribute.md)\<``null`` \| `number`, `any`\> ; `supportedModes`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `label`: [`FieldType`](tlv_export.FieldType.md)\<`string`\> ; `mode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\> ; `semanticTags`: [`FieldType`](tlv_export.FieldType.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<...\>[]\>  }\>[], `any`\>  } ; `commands`: \{ `changeToMode`: [`Command`](cluster_export.Command.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `newMode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\>  }\>, `void`, `any`\>  } = Cluster.commands; `features`: \{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  } = Cluster.features; `id`: [`Branded`](../modules/util_export.md#branded)\<``80``, ``"ClusterId"``\> = Cluster.id; `name`: ``"ModeSelect"`` = Cluster.name; `revision`: ``1`` = Cluster.revision }\>, `ValuesT`\>

#### Inherited from

Identity.set

#### Defined in

[packages/matter.js/src/cluster/mutation/MutableCluster.ts:81](https://github.com/project-chip/matter.js/blob/3adaded6/packages/matter.js/src/cluster/mutation/MutableCluster.ts#L81)

___

### with

▸ **with**\<`SelectionT`\>(`...selection`): [`Of`](cluster_export.ClusterType.Of.md)\<\{ `attributes`: \{ `acceptedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `attributeList`: [`Attribute`](cluster_export.Attribute.md)\<[`AttributeId`](../modules/datatype_export.md#attributeid)[], `never`\> ; `clusterRevision`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `never`\> ; `currentMode`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `any`\> ; `description`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<`string`, `any`\> ; `eventList`: [`Attribute`](cluster_export.Attribute.md)\<[`EventId`](../modules/datatype_export.md#eventid)[], `never`\> ; `featureMap`: [`Attribute`](cluster_export.Attribute.md)\<[`TypeFromPartialBitSchema`](../modules/schema_export.md#typefrompartialbitschema)\<\{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  }\>, `never`\> ; `generatedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `onMode`: [`WritableAttribute`](cluster_export.WritableAttribute.md)\<``null`` \| `number`, `any`\> & \{ `isConditional`: ``true`` = true; `mandatoryIf`: [] \| [\{ `onOff`: `boolean` = true }] ; `optional`: ``true`` = true; `optionalIf`: [] \| [`ConditionalFeatureList`](../modules/cluster_export.md#conditionalfeaturelist)\<[`BitSchema`](../modules/schema_export.md#bitschema)\>  } ; `standardNamespace`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<``null`` \| `number`, `any`\> ; `startUpMode`: [`OptionalWritableAttribute`](cluster_export.OptionalWritableAttribute.md)\<``null`` \| `number`, `any`\> ; `supportedModes`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `label`: [`FieldType`](tlv_export.FieldType.md)\<`string`\> ; `mode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\> ; `semanticTags`: [`FieldType`](tlv_export.FieldType.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `mfgCode`: ... ; `value`: ...  }\>[]\>  }\>[], `any`\>  } ; `commands`: \{ `changeToMode`: [`Command`](cluster_export.Command.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `newMode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\>  }\>, `void`, `any`\>  } = Cluster.commands; `features`: \{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  } = Cluster.features; `id`: [`Branded`](../modules/util_export.md#branded)\<``80``, ``"ClusterId"``\> = Cluster.id; `name`: ``"ModeSelect"`` = Cluster.name; `revision`: ``1`` = Cluster.revision }\>

Select features using [ClusterComposer.compose](../classes/cluster_export.ClusterComposer-1.md#compose).

#### Type parameters

| Name | Type |
| :------ | :------ |
| `SelectionT` | extends [`FeatureSelection`](../modules/cluster_export.ClusterComposer.md#featureselection)\<[`Of`](cluster_export.ClusterType.Of.md)\<\{ `attributes`: \{ `acceptedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `attributeList`: [`Attribute`](cluster_export.Attribute.md)\<[`AttributeId`](../modules/datatype_export.md#attributeid)[], `never`\> ; `clusterRevision`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `never`\> ; `currentMode`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `any`\> ; `description`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<`string`, `any`\> ; `eventList`: [`Attribute`](cluster_export.Attribute.md)\<[`EventId`](../modules/datatype_export.md#eventid)[], `never`\> ; `featureMap`: [`Attribute`](cluster_export.Attribute.md)\<[`TypeFromPartialBitSchema`](../modules/schema_export.md#typefrompartialbitschema)\<\{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  }\>, `never`\> ; `generatedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `onMode`: [`WritableAttribute`](cluster_export.WritableAttribute.md)\<``null`` \| `number`, `any`\> & \{ `isConditional`: ``true`` = true; `mandatoryIf`: [] \| [\{ `onOff`: `boolean` = true }] ; `optional`: ``true`` = true; `optionalIf`: [] \| [`ConditionalFeatureList`](../modules/cluster_export.md#conditionalfeaturelist)\<[`BitSchema`](../modules/schema_export.md#bitschema)\>  } ; `standardNamespace`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<``null`` \| `number`, `any`\> ; `startUpMode`: [`OptionalWritableAttribute`](cluster_export.OptionalWritableAttribute.md)\<``null`` \| `number`, `any`\> ; `supportedModes`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `label`: [`FieldType`](tlv_export.FieldType.md)\<`string`\> ; `mode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\> ; `semanticTags`: [`FieldType`](tlv_export.FieldType.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<...\>[]\>  }\>[], `any`\>  } ; `commands`: \{ `changeToMode`: [`Command`](cluster_export.Command.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `newMode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\>  }\>, `void`, `any`\>  } = Cluster.commands; `features`: \{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  } = Cluster.features; `id`: [`Branded`](../modules/util_export.md#branded)\<``80``, ``"ClusterId"``\> = Cluster.id; `name`: ``"ModeSelect"`` = Cluster.name; `revision`: ``1`` = Cluster.revision }\>\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `...selection` | `SelectionT` |

#### Returns

[`Of`](cluster_export.ClusterType.Of.md)\<\{ `attributes`: \{ `acceptedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `attributeList`: [`Attribute`](cluster_export.Attribute.md)\<[`AttributeId`](../modules/datatype_export.md#attributeid)[], `never`\> ; `clusterRevision`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `never`\> ; `currentMode`: [`Attribute`](cluster_export.Attribute.md)\<`number`, `any`\> ; `description`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<`string`, `any`\> ; `eventList`: [`Attribute`](cluster_export.Attribute.md)\<[`EventId`](../modules/datatype_export.md#eventid)[], `never`\> ; `featureMap`: [`Attribute`](cluster_export.Attribute.md)\<[`TypeFromPartialBitSchema`](../modules/schema_export.md#typefrompartialbitschema)\<\{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  }\>, `never`\> ; `generatedCommandList`: [`Attribute`](cluster_export.Attribute.md)\<[`CommandId`](../modules/datatype_export.md#commandid)[], `never`\> ; `onMode`: [`WritableAttribute`](cluster_export.WritableAttribute.md)\<``null`` \| `number`, `any`\> & \{ `isConditional`: ``true`` = true; `mandatoryIf`: [] \| [\{ `onOff`: `boolean` = true }] ; `optional`: ``true`` = true; `optionalIf`: [] \| [`ConditionalFeatureList`](../modules/cluster_export.md#conditionalfeaturelist)\<[`BitSchema`](../modules/schema_export.md#bitschema)\>  } ; `standardNamespace`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<``null`` \| `number`, `any`\> ; `startUpMode`: [`OptionalWritableAttribute`](cluster_export.OptionalWritableAttribute.md)\<``null`` \| `number`, `any`\> ; `supportedModes`: [`FixedAttribute`](cluster_export.FixedAttribute.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `label`: [`FieldType`](tlv_export.FieldType.md)\<`string`\> ; `mode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\> ; `semanticTags`: [`FieldType`](tlv_export.FieldType.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `mfgCode`: ... ; `value`: ...  }\>[]\>  }\>[], `any`\>  } ; `commands`: \{ `changeToMode`: [`Command`](cluster_export.Command.md)\<[`TypeFromFields`](../modules/tlv_export.md#typefromfields)\<\{ `newMode`: [`FieldType`](tlv_export.FieldType.md)\<`number`\>  }\>, `void`, `any`\>  } = Cluster.commands; `features`: \{ `onOff`: [`BitFlag`](../modules/schema_export.md#bitflag)  } = Cluster.features; `id`: [`Branded`](../modules/util_export.md#branded)\<``80``, ``"ClusterId"``\> = Cluster.id; `name`: ``"ModeSelect"`` = Cluster.name; `revision`: ``1`` = Cluster.revision }\>

#### Inherited from

Identity.with

#### Defined in

[packages/matter.js/src/cluster/mutation/MutableCluster.ts:67](https://github.com/project-chip/matter.js/blob/3adaded6/packages/matter.js/src/cluster/mutation/MutableCluster.ts#L67)