## API Report File for "components-srcs"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { AfterViewInit } from '@angular/core';
import { AnimationTriggerMetadata } from '@angular/animations';
import { AriaDescriber } from '@angular/cdk/a11y';
import { BooleanInput } from '@angular/cdk/coercion';
import { ChangeDetectorRef } from '@angular/core';
import { ComponentType } from '@angular/cdk/overlay';
import { ConnectedPosition } from '@angular/cdk/overlay';
import { Directionality } from '@angular/cdk/bidi';
import { ElementRef } from '@angular/core';
import { FocusMonitor } from '@angular/cdk/a11y';
import * as i0 from '@angular/core';
import * as i2 from '@angular/cdk/a11y';
import * as i3 from '@angular/common';
import * as i4 from '@angular/cdk/overlay';
import * as i5 from '@angular/material/core';
import * as i6 from '@angular/cdk/scrolling';
import { InjectionToken } from '@angular/core';
import { NgZone } from '@angular/core';
import { NumberInput } from '@angular/cdk/coercion';
import { Observable } from 'rxjs';
import { OnDestroy } from '@angular/core';
import { OriginConnectionPosition } from '@angular/cdk/overlay';
import { Overlay } from '@angular/cdk/overlay';
import { OverlayConnectionPosition } from '@angular/cdk/overlay';
import { OverlayRef } from '@angular/cdk/overlay';
import { Platform } from '@angular/cdk/platform';
import { ScrollDispatcher } from '@angular/cdk/overlay';
import { ScrollStrategy } from '@angular/cdk/overlay';
import { ViewContainerRef } from '@angular/core';

// @public
export function getMatTooltipInvalidPositionError(position: string): Error;

// @public
export const MAT_TOOLTIP_DEFAULT_OPTIONS: InjectionToken<MatTooltipDefaultOptions>;

// @public
export function MAT_TOOLTIP_DEFAULT_OPTIONS_FACTORY(): MatTooltipDefaultOptions;

// @public
export const MAT_TOOLTIP_SCROLL_STRATEGY: InjectionToken<() => ScrollStrategy>;

// @public
export function MAT_TOOLTIP_SCROLL_STRATEGY_FACTORY(overlay: Overlay): () => ScrollStrategy;

// @public
export const MAT_TOOLTIP_SCROLL_STRATEGY_FACTORY_PROVIDER: {
    provide: InjectionToken<() => ScrollStrategy>;
    deps: (typeof Overlay)[];
    useFactory: typeof MAT_TOOLTIP_SCROLL_STRATEGY_FACTORY;
};

// @public
export class MatTooltip extends _MatTooltipBase<TooltipComponent> {
    constructor(overlay: Overlay, elementRef: ElementRef<HTMLElement>, scrollDispatcher: ScrollDispatcher, viewContainerRef: ViewContainerRef, ngZone: NgZone, platform: Platform, ariaDescriber: AriaDescriber, focusMonitor: FocusMonitor, scrollStrategy: any, dir: Directionality, defaultOptions: MatTooltipDefaultOptions, _document: any);
    // (undocumented)
    protected _addOffset(position: ConnectedPosition): ConnectedPosition;
    // (undocumented)
    protected readonly _cssClassPrefix = "mat-mdc";
    // (undocumented)
    protected readonly _tooltipComponent: typeof TooltipComponent;
    // (undocumented)
    static ɵdir: i0.ɵɵDirectiveDeclaration<MatTooltip, "[matTooltip]", ["matTooltip"], {}, {}, never, never, false, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatTooltip, [null, null, null, null, null, null, null, null, null, { optional: true; }, { optional: true; }, null]>;
}

// @public
export const matTooltipAnimations: {
    readonly tooltipState: AnimationTriggerMetadata;
};

// @public (undocumented)
export abstract class _MatTooltipBase<T extends _TooltipComponentBase> implements OnDestroy, AfterViewInit {
    constructor(_overlay: Overlay, _elementRef: ElementRef<HTMLElement>, _scrollDispatcher: ScrollDispatcher, _viewContainerRef: ViewContainerRef, _ngZone: NgZone, _platform: Platform, _ariaDescriber: AriaDescriber, _focusMonitor: FocusMonitor, scrollStrategy: any, _dir: Directionality, _defaultOptions: MatTooltipDefaultOptions, _document: any);
    protected _addOffset(position: ConnectedPosition): ConnectedPosition;
    // (undocumented)
    protected readonly _cssClassPrefix: string;
    // (undocumented)
    protected _dir: Directionality;
    get disabled(): boolean;
    set disabled(value: BooleanInput);
    _getOrigin(): {
        main: OriginConnectionPosition;
        fallback: OriginConnectionPosition;
    };
    _getOverlayPosition(): {
        main: OverlayConnectionPosition;
        fallback: OverlayConnectionPosition;
    };
    hide(delay?: number): void;
    get hideDelay(): number;
    set hideDelay(value: NumberInput);
    _isTooltipVisible(): boolean;
    get message(): string;
    set message(value: string);
    // (undocumented)
    ngAfterViewInit(): void;
    ngOnDestroy(): void;
    // (undocumented)
    _overlayRef: OverlayRef | null;
    get position(): TooltipPosition;
    set position(value: TooltipPosition);
    // (undocumented)
    get positionAtOrigin(): boolean;
    set positionAtOrigin(value: BooleanInput);
    show(delay?: number, origin?: {
        x: number;
        y: number;
    }): void;
    get showDelay(): number;
    set showDelay(value: NumberInput);
    toggle(origin?: {
        x: number;
        y: number;
    }): void;
    get tooltipClass(): string | string[] | Set<string> | {
        [key: string]: any;
    };
    set tooltipClass(value: string | string[] | Set<string> | {
        [key: string]: any;
    });
    // (undocumented)
    protected abstract readonly _tooltipComponent: ComponentType<T>;
    // (undocumented)
    _tooltipInstance: T | null;
    touchGestures: TooltipTouchGestures;
    // (undocumented)
    protected _viewportMargin: number;
    // (undocumented)
    static ɵdir: i0.ɵɵDirectiveDeclaration<_MatTooltipBase<any>, never, never, { "position": "matTooltipPosition"; "positionAtOrigin": "matTooltipPositionAtOrigin"; "disabled": "matTooltipDisabled"; "showDelay": "matTooltipShowDelay"; "hideDelay": "matTooltipHideDelay"; "touchGestures": "matTooltipTouchGestures"; "message": "matTooltip"; "tooltipClass": "matTooltipClass"; }, {}, never, never, false, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<_MatTooltipBase<any>, never>;
}

// @public
export interface MatTooltipDefaultOptions {
    disableTooltipInteractivity?: boolean;
    hideDelay: number;
    position?: TooltipPosition;
    positionAtOrigin?: boolean;
    showDelay: number;
    touchendHideDelay: number;
    touchGestures?: TooltipTouchGestures;
}

// @public (undocumented)
export class MatTooltipModule {
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatTooltipModule, never>;
    // (undocumented)
    static ɵinj: i0.ɵɵInjectorDeclaration<MatTooltipModule>;
    // (undocumented)
    static ɵmod: i0.ɵɵNgModuleDeclaration<MatTooltipModule, [typeof i1.MatTooltip, typeof i1.TooltipComponent], [typeof i2.A11yModule, typeof i3.CommonModule, typeof i4.OverlayModule, typeof i5.MatCommonModule], [typeof i1.MatTooltip, typeof i1.TooltipComponent, typeof i5.MatCommonModule, typeof i6.CdkScrollableModule]>;
}

// @public
export const SCROLL_THROTTLE_MS = 20;

// @public @deprecated
export const TOOLTIP_PANEL_CLASS = "mat-mdc-tooltip-panel";

// @public
export class TooltipComponent extends _TooltipComponentBase {
    constructor(changeDetectorRef: ChangeDetectorRef, _elementRef: ElementRef<HTMLElement>, animationMode?: string);
    // (undocumented)
    _hideAnimation: string;
    // (undocumented)
    _isMultiline: boolean;
    // (undocumented)
    protected _onShow(): void;
    // (undocumented)
    _showAnimation: string;
    _tooltip: ElementRef<HTMLElement>;
    // (undocumented)
    static ɵcmp: i0.ɵɵComponentDeclaration<TooltipComponent, "mat-tooltip-component", never, {}, {}, never, never, false, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<TooltipComponent, [null, null, { optional: true; }]>;
}

// @public (undocumented)
export abstract class _TooltipComponentBase implements OnDestroy {
    constructor(_changeDetectorRef: ChangeDetectorRef, animationMode?: string);
    afterHidden(): Observable<void>;
    _cancelPendingAnimations(): void;
    _handleAnimationEnd({ animationName }: AnimationEvent): void;
    _handleBodyInteraction(): void;
    // (undocumented)
    _handleMouseLeave({ relatedTarget }: MouseEvent): void;
    hide(delay: number): void;
    protected abstract readonly _hideAnimation: string;
    isVisible(): boolean;
    _markForCheck(): void;
    message: string;
    _mouseLeaveHideDelay: number;
    // (undocumented)
    ngOnDestroy(): void;
    protected _onShow(): void;
    show(delay: number): void;
    protected abstract readonly _showAnimation: string;
    abstract _tooltip: ElementRef<HTMLElement>;
    tooltipClass: string | string[] | Set<string> | {
        [key: string]: any;
    };
    _triggerElement: HTMLElement;
    // (undocumented)
    static ɵdir: i0.ɵɵDirectiveDeclaration<_TooltipComponentBase, never, never, {}, {}, never, never, false, never>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<_TooltipComponentBase, [null, { optional: true; }]>;
}

// @public
export type TooltipPosition = 'left' | 'right' | 'above' | 'below' | 'before' | 'after';

// @public
export type TooltipTouchGestures = 'auto' | 'on' | 'off';

// @public
export type TooltipVisibility = 'initial' | 'visible' | 'hidden';

// (No @packageDocumentation comment for this package)

```
