## API Report File for "components-srcs"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { AfterContentChecked } from '@angular/core';
import { AfterContentInit } from '@angular/core';
import { AnimationEvent as AnimationEvent_2 } from '@angular/animations';
import { AnimationTriggerMetadata } from '@angular/animations';
import { BooleanInput } from '@angular/cdk/coercion';
import { CdkScrollable } from '@angular/cdk/scrolling';
import { ChangeDetectorRef } from '@angular/core';
import { Directionality } from '@angular/cdk/bidi';
import { DoCheck } from '@angular/core';
import { ElementRef } from '@angular/core';
import { EventEmitter } from '@angular/core';
import { FocusMonitor } from '@angular/cdk/a11y';
import { FocusOrigin } from '@angular/cdk/a11y';
import { FocusTrapFactory } from '@angular/cdk/a11y';
import * as i0 from '@angular/core';
import * as i3 from '@angular/common';
import * as i4 from '@angular/material/core';
import * as i5 from '@angular/cdk/platform';
import * as i6 from '@angular/cdk/scrolling';
import { InjectionToken } from '@angular/core';
import { NgZone } from '@angular/core';
import { NumberInput } from '@angular/cdk/coercion';
import { Observable } from 'rxjs';
import { OnDestroy } from '@angular/core';
import { Platform } from '@angular/cdk/platform';
import { QueryList } from '@angular/core';
import { ScrollDispatcher } from '@angular/cdk/scrolling';
import { Subject } from 'rxjs';
import { ViewportRuler } from '@angular/cdk/scrolling';

// @public
const MAT_DRAWER_CONTAINER: InjectionToken<unknown>;

// @public
export const MAT_DRAWER_DEFAULT_AUTOSIZE: InjectionToken<boolean>;

// @public
export function MAT_DRAWER_DEFAULT_AUTOSIZE_FACTORY(): boolean;

// @public
export class MatDrawer implements AfterContentInit, AfterContentChecked, OnDestroy {
    constructor(_elementRef: ElementRef<HTMLElement>, _focusTrapFactory: FocusTrapFactory, _focusMonitor: FocusMonitor, _platform: Platform, _ngZone: NgZone, _doc: any, _container?: MatDrawerContainer | undefined);
    // (undocumented)
    _animationDoneListener(event: AnimationEvent_2): void;
    readonly _animationEnd: Subject<AnimationEvent_2>;
    readonly _animationStarted: Subject<AnimationEvent_2>;
    // (undocumented)
    _animationStartListener(event: AnimationEvent_2): void;
    _animationState: 'open-instant' | 'open' | 'void';
    get autoFocus(): boolean;
    set autoFocus(value: boolean);
    close(): Promise<MatDrawerToggleResult>;
    readonly closedStart: Observable<void>;
    readonly _closedStream: Observable<void>;
    _closeViaBackdropClick(): Promise<MatDrawerToggleResult>;
    // (undocumented)
    _container?: MatDrawerContainer | undefined;
    get disableClose(): boolean;
    set disableClose(value: boolean);
    // (undocumented)
    _getWidth(): number;
    get mode(): MatDrawerMode;
    set mode(value: MatDrawerMode);
    readonly _modeChanged: Subject<void>;
    // (undocumented)
    static ngAcceptInputType_autoFocus: BooleanInput;
    // (undocumented)
    static ngAcceptInputType_disableClose: BooleanInput;
    // (undocumented)
    static ngAcceptInputType_opened: BooleanInput;
    // (undocumented)
    ngAfterContentChecked(): void;
    // (undocumented)
    ngAfterContentInit(): void;
    // (undocumented)
    ngOnDestroy(): void;
    readonly onPositionChanged: EventEmitter<void>;
    open(openedVia?: FocusOrigin): Promise<MatDrawerToggleResult>;
    get opened(): boolean;
    set opened(value: boolean);
    readonly openedChange: EventEmitter<boolean>;
    readonly openedStart: Observable<void>;
    readonly _openedStream: Observable<void>;
    get position(): 'start' | 'end';
    set position(value: 'start' | 'end');
    toggle(isOpen?: boolean, openedVia?: FocusOrigin): Promise<MatDrawerToggleResult>;
    // (undocumented)
    static ɵcmp: i0.ɵɵComponentDeclaration<MatDrawer, "mat-drawer", ["matDrawer"], { "position": "position"; "mode": "mode"; "disableClose": "disableClose"; "autoFocus": "autoFocus"; "opened": "opened"; }, { "openedChange": "openedChange"; "_openedStream": "opened"; "openedStart": "openedStart"; "_closedStream": "closed"; "closedStart": "closedStart"; "onPositionChanged": "positionChanged"; }, never, ["*"]>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatDrawer, [null, null, null, null, null, { optional: true; }, { optional: true; }]>;
}

// @public
export const matDrawerAnimations: {
    readonly transformDrawer: AnimationTriggerMetadata;
};

// @public
export class MatDrawerContainer implements AfterContentInit, DoCheck, OnDestroy {
    constructor(_dir: Directionality, _element: ElementRef<HTMLElement>, _ngZone: NgZone, _changeDetectorRef: ChangeDetectorRef, viewportRuler: ViewportRuler, defaultAutosize?: boolean, _animationMode?: string | undefined);
    _allDrawers: QueryList<MatDrawer>;
    get autosize(): boolean;
    set autosize(value: boolean);
    readonly backdropClick: EventEmitter<void>;
    // (undocumented)
    _backdropOverride: boolean | null;
    close(): void;
    // (undocumented)
    _closeModalDrawersViaBackdrop(): void;
    // (undocumented)
    _content: MatDrawerContent;
    // (undocumented)
    readonly _contentMarginChanges: Subject<{
        left: number | null;
        right: number | null;
    }>;
    _contentMargins: {
        left: number | null;
        right: number | null;
    };
    _drawers: QueryList<MatDrawer>;
    get end(): MatDrawer | null;
    get hasBackdrop(): any;
    set hasBackdrop(value: any);
    // (undocumented)
    _isShowingBackdrop(): boolean;
    // (undocumented)
    static ngAcceptInputType_autosize: BooleanInput;
    // (undocumented)
    static ngAcceptInputType_hasBackdrop: BooleanInput;
    // (undocumented)
    ngAfterContentInit(): void;
    // (undocumented)
    ngDoCheck(): void;
    // (undocumented)
    ngOnDestroy(): void;
    // (undocumented)
    _onBackdropClicked(): void;
    open(): void;
    get scrollable(): CdkScrollable;
    get start(): MatDrawer | null;
    updateContentMargins(): void;
    // (undocumented)
    _userContent: MatDrawerContent;
    // (undocumented)
    static ɵcmp: i0.ɵɵComponentDeclaration<MatDrawerContainer, "mat-drawer-container", ["matDrawerContainer"], { "autosize": "autosize"; "hasBackdrop": "hasBackdrop"; }, { "backdropClick": "backdropClick"; }, ["_content", "_allDrawers"], ["mat-drawer", "mat-drawer-content", "*"]>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatDrawerContainer, [{ optional: true; }, null, null, null, null, null, { optional: true; }]>;
}

// @public (undocumented)
export class MatDrawerContent extends CdkScrollable implements AfterContentInit {
    constructor(_changeDetectorRef: ChangeDetectorRef, _container: MatDrawerContainer, elementRef: ElementRef<HTMLElement>, scrollDispatcher: ScrollDispatcher, ngZone: NgZone);
    // (undocumented)
    _container: MatDrawerContainer;
    // (undocumented)
    ngAfterContentInit(): void;
    // (undocumented)
    static ɵcmp: i0.ɵɵComponentDeclaration<MatDrawerContent, "mat-drawer-content", never, {}, {}, never, ["*"]>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatDrawerContent, never>;
}

// @public
export type MatDrawerMode = 'over' | 'push' | 'side';

// @public
export type MatDrawerToggleResult = 'open' | 'close';

// @public (undocumented)
export class MatSidenav extends MatDrawer {
    get fixedBottomGap(): number;
    set fixedBottomGap(value: number);
    get fixedInViewport(): boolean;
    set fixedInViewport(value: boolean);
    get fixedTopGap(): number;
    set fixedTopGap(value: number);
    // (undocumented)
    static ngAcceptInputType_fixedBottomGap: NumberInput;
    // (undocumented)
    static ngAcceptInputType_fixedInViewport: BooleanInput;
    // (undocumented)
    static ngAcceptInputType_fixedTopGap: NumberInput;
    // (undocumented)
    static ɵcmp: i0.ɵɵComponentDeclaration<MatSidenav, "mat-sidenav", ["matSidenav"], { "fixedInViewport": "fixedInViewport"; "fixedTopGap": "fixedTopGap"; "fixedBottomGap": "fixedBottomGap"; }, {}, never, ["*"]>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatSidenav, never>;
}

// @public (undocumented)
export class MatSidenavContainer extends MatDrawerContainer {
    // (undocumented)
    _allDrawers: QueryList<MatSidenav>;
    // (undocumented)
    _content: MatSidenavContent;
    // (undocumented)
    static ɵcmp: i0.ɵɵComponentDeclaration<MatSidenavContainer, "mat-sidenav-container", ["matSidenavContainer"], {}, {}, ["_content", "_allDrawers"], ["mat-sidenav", "mat-sidenav-content", "*"]>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatSidenavContainer, never>;
}

// @public (undocumented)
export class MatSidenavContent extends MatDrawerContent {
    constructor(changeDetectorRef: ChangeDetectorRef, container: MatSidenavContainer, elementRef: ElementRef<HTMLElement>, scrollDispatcher: ScrollDispatcher, ngZone: NgZone);
    // (undocumented)
    static ɵcmp: i0.ɵɵComponentDeclaration<MatSidenavContent, "mat-sidenav-content", never, {}, {}, never, ["*"]>;
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatSidenavContent, never>;
}

// @public (undocumented)
export class MatSidenavModule {
    // (undocumented)
    static ɵfac: i0.ɵɵFactoryDeclaration<MatSidenavModule, never>;
    // (undocumented)
    static ɵinj: i0.ɵɵInjectorDeclaration<MatSidenavModule>;
    // (undocumented)
    static ɵmod: i0.ɵɵNgModuleDeclaration<MatSidenavModule, [typeof i1.MatDrawer, typeof i1.MatDrawerContainer, typeof i1.MatDrawerContent, typeof i2.MatSidenav, typeof i2.MatSidenavContainer, typeof i2.MatSidenavContent], [typeof i3.CommonModule, typeof i4.MatCommonModule, typeof i5.PlatformModule, typeof i6.CdkScrollableModule], [typeof i6.CdkScrollableModule, typeof i4.MatCommonModule, typeof i1.MatDrawer, typeof i1.MatDrawerContainer, typeof i1.MatDrawerContent, typeof i2.MatSidenav, typeof i2.MatSidenavContainer, typeof i2.MatSidenavContent]>;
}

// @public
export function throwMatDuplicatedDrawerError(position: string): void;

// (No @packageDocumentation comment for this package)

```