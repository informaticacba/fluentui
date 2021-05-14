## API Report File for "@fluentui/react-badge"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts

import { ComponentProps } from '@fluentui/react-utilities';
import { ObjectShorthandProps } from '@fluentui/react-utilities';
import * as React_2 from 'react';
import { ShorthandProps } from '@fluentui/react-utilities';

// @public
export const Badge: React_2.FunctionComponent<BadgeProps & React_2.RefAttributes<HTMLElement>>;

// @public (undocumented)
export type BadgeAppearance = 'filled' | 'outline' | 'ghost' | 'tint';

// @public (undocumented)
export interface BadgeProps extends ComponentProps, React_2.HTMLAttributes<HTMLElement> {
    appearance?: BadgeAppearance;
    icon?: ShorthandProps<React_2.HTMLAttributes<HTMLElement>>;
    iconPosition?: 'before' | 'after';
    shape?: BadgeShape;
    size?: BadgeSize;
}

// @public (undocumented)
export type BadgeShape = 'rounded' | 'square' | 'circular';

// @public
export const badgeShorthandProps: readonly ["icon"];

// @public (undocumented)
export type BadgeSize = 'smallest' | 'smaller' | 'small' | 'medium' | 'large' | 'larger' | 'largest';

// @public (undocumented)
export interface BadgeState extends BadgeProps {
    icon?: ObjectShorthandProps<React_2.HTMLAttributes<HTMLSpanElement>>;
    ref: React_2.RefObject<HTMLElement>;
}

// @public
export const CounterBadge: React_2.ForwardRefExoticComponent<CounterBadgeProps & React_2.RefAttributes<HTMLElement>>;

// @public (undocumented)
export type CounterBadgeColors = 'accent' | 'warning' | 'important' | 'severe' | 'informative';

// @public (undocumented)
export interface CounterBadgeProps extends Omit<BadgeProps, 'appearance' | 'shape'> {
    appearance?: Extract<BadgeProps['appearance'], 'filled' | 'ghost'>;
    color?: CounterBadgeColors;
    count?: number;
    dot?: boolean;
    overflowCount?: number;
    shape?: Extract<BadgeProps['shape'], 'rounded' | 'circular'>;
    showZero?: boolean;
}

// @public
export const counterBadgeShorthandProps: readonly ["icon"];

// @public (undocumented)
export interface CounterBadgeState extends BadgeState {
    count: number;
    dot: boolean;
    overflowCount: number;
    showZero: boolean;
}

// @public
export const PresenceBadge: React_2.ForwardRefExoticComponent<PresenceBadgeProps & React_2.RefAttributes<HTMLElement>>;

// @public (undocumented)
export interface PresenceBadgeProps extends Omit<BadgeProps, 'shape' | 'appearance'> {
    outOfOffice?: boolean;
    status?: PresenceBadgeStatus;
}

// @public
export const presenceBadgeShorthandProps: (keyof PresenceBadgeProps)[];

// @public (undocumented)
export interface PresenceBadgeState extends Omit<BadgeState, 'shape' | 'appearance'> {
    outOfOffice: boolean;
    status: PresenceBadgeStatus;
}

// @public (undocumented)
export type PresenceBadgeStatus = 'busy' | 'outOfOffice' | 'away' | 'available' | 'offline' | 'doNotDisturb';

// @public (undocumented)
export const renderBadge: (state: BadgeState) => JSX.Element;

// @public
export const useBadge: (props: BadgeProps, ref: React_2.Ref<HTMLElement>, defaultProps?: BadgeProps | undefined) => BadgeState;

// @public
export const useBadgeStyles: (state: BadgeState) => BadgeState;

// @public
export const useCounterBadge: (props: CounterBadgeProps, ref: React_2.Ref<HTMLElement>, defaultProps?: CounterBadgeProps | undefined) => CounterBadgeState;

// @public
export const useCounterBadgeStyles: (state: CounterBadgeState) => CounterBadgeState;

// @public
export const usePresenceBadge: (props: PresenceBadgeProps, ref: React_2.Ref<HTMLElement>, defaultProps?: PresenceBadgeProps | undefined) => PresenceBadgeState;

// @public
export const usePresenceBadgeStyles: (state: PresenceBadgeState) => PresenceBadgeState;


// (No @packageDocumentation comment for this package)

```